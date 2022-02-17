<template>
  <div class="home">
  <div class="user">
    <img v-bind:src="'https://i.pinimg.com/750x/3e/2e/8c/3e2e8c6fa626636eb4e8bdfe78edab3b.jpg'" alt="profile picture">
      <p>Mary-Beth</p>
      <p id="logout">Log Out</p>
  </div>
    <post_compo  :postsList="postsList"> </post_compo>
  </div>
</template>

<script>

import post_compo from "@/components/post_compo.vue";


export default {
  name: "posts",
  components: {
    post_compo,
  },
  props: ["postsList"],
 data(){
 return{
 }},
 methods: {}
};

</script>

<style scoped>
.home {
background-color: rgb(223, 213, 220);
}

.user {
  text-align: center;
  position: fixed;
  height: 100%;
  width: 140px;
  background-color: rgb(255, 255, 255);
  padding: 10px;
}

.user p {
  color: rgb(31, 31, 31);
  font-weight: bold;
}

.user #logout {
  color:rgb(124, 124, 124);
  font-weight: 200;
  font-size: 14px;
}

.user img {
  width: 100px;
  height: 100px;
  object-fit: cover;
  border-radius: 50%;
}

.post {
  width: 70%;
  border-radius: 1px;
  margin: 10px;
  box-shadow: 5px 5px 20px 3px rgb(151, 151, 151);
  margin-top: 60px;
  display: flex;
  flex-direction: column;
}

</style>
