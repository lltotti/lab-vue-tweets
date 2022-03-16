<template>
  <img :src="image" className="profile" alt="profile"/>
  
</template>



<script>
export default {
   props: {
    image: {
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
