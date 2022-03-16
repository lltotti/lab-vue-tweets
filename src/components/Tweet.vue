<template>
  <div className="tweet">
    <ProfileImage :image="tweets.user.image" />
    <div className="body">
      <div className="top">
        <User :userData="tweets.user"/>
        <Timestamp :timestamp="tweets.timestamp"/>
      </div>
      <Message :message="tweets.message"/>
      <Actions />

    </div>
  

  </div>
</template>



<script>
import ProfileImage from "../components/ProfileImage.vue";
import User from "../components/User.vue";
import Timestamp from "../components/Timestamp.vue";
import Message from "../components/Message.vue";
import Actions from "../components/Actions.vue";

export default {
   components: {
     ProfileImage,
     User,
     Timestamp,
     Message,
     Actions
   },
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
