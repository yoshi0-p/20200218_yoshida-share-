<template>
  <div class = "frame">
    <div class="left-padding">
      <h1>Memo+</h1>
      <div class="flex icon-field" @click="$router.push('/home')">
        <p>ホーム</p>
      </div>
      <div class="flex icon-field" @click="$router.push('/profile')">
        <p>プロフィール</p>
      </div>
      <div class="flex icon-field" @click="$store.dispatch('logout')">
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
  border:black;
}
.left-padding {
  margin: 20px;
}
.flex {
  display: flex;
}
.logo {
  width: 100px;
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