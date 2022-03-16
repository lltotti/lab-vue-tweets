<template>
   <span className="user">
          <span className="name">{{userData.name}}</span>
          <span className="handle">{{userData.handle}}</span>
  </span>
</template>




<script>
export default {
   props: {
    userData: {
      type: Object,
      default:{
        name: "none",
        handle: "none"
      }
    },
  }
}

</script>




<style scoped>
a {
  color: #42b983;
}
</style>
