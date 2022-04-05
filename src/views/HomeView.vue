<template>

<div class="postbox">
   <h2> <strong> News Feed </strong>  </h2>
   <br>
    <PostItems v-for="post of posts" :post="post" :key="post.url" />
              </div>
 
  
</template>

<script>
import PostItems from "../components/PostItems.vue"
export default {

  components: { PostItems },

  data() {
    return {
  posts: [],
    };
  },

  mounted() {
    fetch("http://localhost:3000")
      .then((res) => res.json())
      .then((data) => {
        console.log(data)
        this.posts = data.data.articles
      });
  },
}

</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
