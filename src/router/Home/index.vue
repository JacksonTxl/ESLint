<template>
  <main>
    <el-button type="primary" @click.native="hello">primary</el-button>
    <hello></hello>
  </main>
</template>

<script>
  import { Button , Message } from 'element-ui' ;
  import Hello from 'components/Hello' ;

  export default {
    components: {
      ElButton: Button ,
      Hello
    } ,
    methods: {
      hello () {
        var m = '1223' ;

        Message(m + 'Hello Vue') ;
        console.log('adfasdfas') ;
      }
    }
  } ;
</script>
