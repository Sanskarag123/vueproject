<template>
  <div class="login">
    <label class="name">Username</label><br>
    <input type="text" name="username" v-model="user.name" >
<br><input type="password" name="password"  v-model="user.password">
 <br>   <button v-on:keyup.enter="submit" v-on:click="submit"> login</button>
  </div>
</template>
<script>
export default {
  name:'login',
  data(){
    return{
    title:'login page',
    user:
      {
       name:undefined,
       password:undefined
      },
      pass1:false
    }
  },
  methods:{
    pass:function()
    {
      pass1=true;
    }
  }
  
}
</script>

<style scoped>
.login{
color:red;
margin:100px;
}

</style>


