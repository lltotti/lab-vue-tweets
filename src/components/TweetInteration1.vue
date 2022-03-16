<template>
  <div className="tweet">
    <img
      :src="tweets.user.image"
      className="profile"
      alt="profile"
    />

    <div className="body">
      <div className="top">
        <span className="user">
          <span className="name">{{tweets.user.name}}</span>
          <span className="handle">{{tweets.user.handle}}</span>
        </span>

        <span className="timestamp">{{tweets.timestamp}}</span>
      </div>

      <p className="message">
        {{tweets.message}}
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>



<script>
export default {
   props: {
    tweets: {
      type: Object,
      default: {
          user: {
                    name: "None",
                    image: "none",
                    handle: "None",
                },
                timestamp: "None",
                message: "None",
            },
    },
  },
}

</script>


<style scoped>
a {
  color: #42b983;
}
</style>
