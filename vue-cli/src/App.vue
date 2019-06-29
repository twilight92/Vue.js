<template>
  <!-- 템플릿 안에는 html엘리먼트가 최상위에 하나만 있어야한다. : 템플릿 루트는 하나여야 한다. -->
  <div>
    <!-- <app-header v-bind:프롭스 속성 이름="상위 컴포넌트의 데이터 이름"></app-header> -->
    <app-header
     v-bind:propsdata="str"
     v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
//import 변수 from '경로/파일' : 파일의 내용 들고온다.
import AppHeader from './components/AppHeader.vue';

/* var AppHeader = {
  template: '<header><h1>Header</h1></header>'
} */

/* 
new Vue({
  data: {
    str: 'hi'
  }
}) 
*/

export default {
  data : function(){
    return {
      str : 'Header'
    }
    //function 내부에 return으로 새 객체 반환해야함
  },
  components: {
    'app-header' : AppHeader
  },
  methods: {
    renewStr: function(){
      this.str = 'hi';
    }
  }
}
</script>

<style>

</style>
