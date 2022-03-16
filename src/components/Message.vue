<template>
  <p className="message"> {{message}} </p> 
  
</template>



<script>
export default {
   props: {
    message: {
      type: String,
      default: "none"
    },
  },
}

</script>


<style scoped>
a {
  color: #42b983;
}
</style>
