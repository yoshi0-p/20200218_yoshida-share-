<template>
  <div class = "frame">
      <h1>付箋ボード</h1>
      <div  class="logout" @click="$store.dispatch('logout')">
        <p>｜ログアウト｜</p>
      </div>
    <ShareMessage />
  </div>
</template>

<script>
import ShareMessage from "../components/ShareMessage";
export default {
  components: {
    ShareMessage
  }
};
</script>

<style scoped>

.frame{
  border-color:black;
  background-color: #977003;
  width:100%;
  height:75px;
  justify-content: center;
  display:flex;
  white-space: nowrap;
}
h1{
  line-height: 75px;
}
.logout{
  line-height: 75px;
}



</style>