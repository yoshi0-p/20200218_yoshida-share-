<template>
  <div class = "frame">
    <div class="left-padding">
      <h1>付箋ボード</h1>
      <div class="icon-field" @click="$store.dispatch('logout')">
        <p>ログアウト</p>
      </div>
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
}

.icon-field {
  margin-top: 15px;
  cursor: pointer;
}
.icon {
  width: 25px;
}
.icon-field p {
  font-size: 16px;
  padding-left: 15px;
}
</style>