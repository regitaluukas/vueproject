<template>
  <div class="home">
  <div class="user">
    <img v-bind:src="'https://upload.wikimedia.org/wikipedia/commons/9/99/Sample_User_Icon.png'" alt="profile picture">
      <p>User Name</p>
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
background-color: rgb(226, 226, 226);
background-image: url("https://storage.googleapis.com/subtlepatterns-production/designers/subtlepatterns/uploads/double-bubble-outline.png");
}

.user {
  text-align: center;
  position: fixed;
  margin: 5px;
  height: 140px;
  width: 140px;
  background-color: rgb(233, 236, 241);
  padding: 10px;
  border-radius: 50%;
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
  width: 60px;
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
