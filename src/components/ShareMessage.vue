<template>
  <div class="share">
    <p>シェア</p>
    <textarea v-model="share"></textarea>
    <div @click="send">
      <button>シェアする</button>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      share: "",
    };
  },
  methods: {
    
    
    
    send() {
      if (this.share === "") {
        alert("シェアする内容を入力してください");
      } else {
        axios
          .post("https://calm-atoll-21933.herokuapp.com/api/shares", {
            user_id: this.$store.state.user.id,
            share: this.share,
          })
          .then((response) => {
            console.log(response);
            alert("シェアしました");
            this.share = "";
            this.$router.go({
              path: this.$router.currentRoute.path,
              force: true,
            });
          });
      }
    },
  },
};
</script>

<style scoped>
.share {
  display:flex;
}
.share textarea {
  width: 95%;
  height: 40px;
  margin-top: 15px;
  margin-bottom: 15px;
  border-radius: 10px;
  border: 1px solid rgb(0, 134, 11);
  background-color: #ffffff;
  color: rgb(0, 0, 0);
  resize: none;
}
button {
  width: 100px;
  text-align: center;
  padding: 8px 0 10px;
  color: #fff;
  background-color: #5419da;
  border-radius: 25px;
  display: block;
  margin: 0 0 0 auto;
}
</style>
