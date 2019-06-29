<template>
  <!-- 템플릿 안에는 html엘리먼트가 최상위에 하나만 있어야한다. : 템플릿 루트는 하나여야 한다. -->
  <div>
    {{ str }}
  </div>
</template>

<script>
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
        str : 'hi'
      }
      //function 내부에 return으로 새 객체 반환해야함
    }
  }
</script>

<style>

</style>
