/*
    컴포넌트 이름은 파스칼케이스로, 최소한 두 단어 이상으로 조합할 것(권고)
    두 단어로 조합하는 이유 : App.vue에서 컴포넌트 가져올 때 컴포넌트 태그인지 html 표준태그인지 브라우저는 알 길이 없음
*/
<template>
    <header>
        <h1>{{ propsdata }}</h1>
    </header>
</template>

<script>
export default {
    props: ['propsdata']
}
</script>

<style>

</style>
