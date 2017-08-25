<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
               <app-quote>
                   <h2>{{ quoteTitle }}</h2>
                   <p>You may delay but time will not</p>
               </app-quote>
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './comp/Quote.vue';

    export default {
        data: function () {
            return {
                quoteTitle: "The quote title passed in data"
            }
        },
        components: {
            appQuote: Quote // nécessaire pour passer app-quote ici
        }
    }
</script>

<style>
</style>
