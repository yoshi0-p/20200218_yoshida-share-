<template>
  <div class="flex">
      <SideNavi />
   
      <div class="title">
        <p>最新５件のメモ
        </p>
      </div>
      <Message />
  </div>
</template>

<script>
import SideNavi from "../components/SideNavi";
import Message from "../components/Message";
export default {
  components: {
    SideNavi,
    Message
  }
};
</script>

<style scoped>

.flex {
  display: flex;
}
.title {
  border-bottom: 1px solid white;
  border-left: 1px solid white;
  padding: 15px;
}
.title p {
  font-size: 20px;
  font-weight: bold;
}
</style>
