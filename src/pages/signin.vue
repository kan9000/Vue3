<template>
  <div>
    <form>
      <div>
        Sign-in
      </div>
      <div>
        <label for="username">Username</label>
        <input type="text" id="username" :value="User1">
      </div>
      <div>
        <label for="password">Password</label>
        <input type="password" id="password" :value="Pass1">
      </div>
      <div>
        <input type="checkbox" id="remember" :checked="check1">
        <label for="remember">Remember username?</label>
      </div>
      <div>
        <button type="button" :disabled="lock">
          Sign-In
        </button>
        <button type="reset" :disabled="lock">
          Reset
        </button>
      </div>
    </form>
  </div>
</template>

<script>
 export default {
   data(){
     return {
       User1:'kanchana',
       Pass1:'1234',
       check1:true,
       lock:false, 
     }
   }
 }
</script>