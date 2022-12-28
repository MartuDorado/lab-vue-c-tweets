<template>
  <div class="tweet">
    <ProfileImage :src= " tweet.user.image"></ProfileImage>

    <div class="body">
      <div class="top">
        <span class="user">
          <User :user = "tweet.user"></User>
        </span>

        <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>

      <Message :message="tweet.message"></Message>

     <Actions></Actions>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';
export default {
  components: {
 ProfileImage,
 Actions,
 User,
 Message,
 Timestamp
  },
  props:{
     tweet: {
      type: Object,
      // required: true,
      default: {
      user: {
        name: "Thoughts of Dog®",
        image: "https://i.imgur.com/b0EdHVV.jpg",
        handle: "dog_feelings",
       },
      timestamp: "1h ago",
      message: "the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company",
    
      }
    }
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
