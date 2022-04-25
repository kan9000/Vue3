<template>
// attribue bind => v-bind:ชื่อแอตทริบิวต์="ชื่อตัวแปร"
// element bind => {{ชื่อตัวแปร}}
// v-html สั่งให้แสดงผลตาม html ในตัวแปร

  <div class="text-bold" :title="name">
    Hello {{name.toUpperCase()}}
    อายุ: {{age}}
    สถานศึกษา : {{school}}
  </div>
  <div>Hello 2 <span v-html="name"></span></div>

  <button :disabled="lock">
    test <b>{{name}}</b>
  </button>
</template>

 //-----------------------------------
 <script>
    export default{
      data(){
        return {
          name:'kanchana',
          // name2:'<i>kanchana</i>',
          age:25,
          school:'วิทยาลัยเทคนิคลพบุรี',
          lock:true,//true or false
        }

      }

    }
 </script>

 //-----------------------------------
 <style>

 </style>