<template>
    <div>
      <div id="navi"><HeaderMenu /></div>
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

}


</style>
