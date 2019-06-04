<template>
    <div class="test">
      <h1>  {{title}}</h1>
      <p v-if="showname">{{user.first_name}}</p>
   
    <button v-on:click="ok">hey</button>
    </div>
</template>
<script>

export default {
    name:'test',
    data(){
        return {
            title: 'hello World',
            user: {
                first_name:'sanskar',
                last_name:'agrawal'
            },
            showname:false
        }
       

            },
             methods: {
            ok:function(){
                alert("hey");

        }
    }
}
</script>


