<template>
 <div class="header flex">
   <div></div>
   <div class="center">
     <h1>Memo+</h1>
   </div>
   <div class="center flex">
     <p @click="$router.push('/signup')">新規登録</p>
     <p>|</p>
     <p @click="$router.push('/')">ログイン</p>
   </div>
 </div>
</template>

<style scoped>
h1{
  color:rgb(25, 133, 34);
  font-size:36px;
  text-shadow:2px,2px,black;
  padding:10px;
}
.right {
 align-items: center;
}
.center{
  cursor: pointer;
}
.right p {
 margin-right: 20px;
 cursor: pointer;
}
.header {
 margin: 20px;
}

.flex {
 display: flex;
 justify-content: space-between;
}
</style>