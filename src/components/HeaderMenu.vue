<template>
  <div class = "frame">
    
      <h1>付箋ボード</h1>
      <div class="icon-field" @click="$store.dispatch('logout')">
        <p>ログアウト</p>
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
  height:40px;
  display:flex;
}


</style>