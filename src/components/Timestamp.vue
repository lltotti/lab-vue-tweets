<template>
  <span className="timestamp">{{timestamp}}</span>
</template>



<script>
export default {
   props: {
    timestamp: {
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
