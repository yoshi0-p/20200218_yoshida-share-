<template>
 <div class="header flex">
   <div class="left">
     <h1>Memo+</h1>
   </div>
   <div class="right flex">
     <p @click="$router.push('/signup')">新規登録</p>
     <p @click="$router.push('/')">ログイン</p>
   </div>
 </div>
</template>

<style scoped>
h1{
  color:white;
  font-size:30px;
}
.right {
 align-items: center;
}
.right p {
 margin-right: 20px;
 cursor: pointer;
}
.header {
 margin: 20px;
}
.logo {
 width: 150px;
 cursor: pointer;
}
.flex {
 display: flex;
 justify-content: space-between;
}
</style>