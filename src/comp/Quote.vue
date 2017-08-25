<template>
  <div>
      <slot class="slot" name="title"></slot> 
      <!-- on lui dit qu'il est 'title' pour dans app -->  
      <hr>
      <slot class="slot" name='content'></slot>  
  </div>
</template>

<script>
    
</script>

<style scoped>
    div {
        border: 1px solid #ccc;
        box-shadow: 1px 1px 2px #333;
        padding: 10px;
        margin: 50px auto;
        text-align: center;
    }
    h2 {
        color: #444;  
    }
    .slot {
        border: 1px red dashed;
    }
</style>
