<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <button @click="selectedComponent = 'appQuote'">Quote</button>
                <button @click="selectedComponent = 'appAuthor'">Author</button>
                <button @click="selectedComponent = 'appNew'">New</button>
                <hr>
                <p>{{ selectedComponent }}</p>
                <component :is="selectedComponent"></component>
               <!-- <app-quote>
                   <h2 slot="title">{{ quoteTitle }}</h2>
                   <p slot="content">You may delay but time will not</p>
               </app-quote> -->
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './comp/Quote.vue';
    import Author from './comp/Author.vue';
    import New from './comp/New.vue';

    export default {
        data: function () {
            return {
                quoteTitle: "Title passed in data",
                selectedComponent: 'app-quote', // appQuote - c'est la valeure défaut
            }
        },
        components: {
            appQuote: Quote, // nécessaire pour passer app-quote ici
            appAuthor:Author,
            appNew: New,
        }
    }
</script>

<style>
</style>
