<template>
    <div>
      <div id="navi"><HeaderMenu /></div>
      <div class="title">
        <p>最新５件のメモ
        </p>
      </div>
      <Message />
      </div>
      

</template>

<script>
import HeaderMenu from "../components/HeaderMenu";
import Message from "../components/Message";
export default {
  components: {
    HeaderMenu,
    Message
  }
};
</script>

<style scoped>

#navi{
  width:100%;
  margin-right:0px;
}
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
