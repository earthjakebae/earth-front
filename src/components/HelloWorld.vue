<template>
  <div class="hello">
    <h1>{{ message }}</h1>
    <h1>환경설정 파일 다수 적용 테스트 두번째</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  computed:{
    message() {
      return process.env.VUE_APP_MESSAGE || 'Default Message';
    }
  }
}
</script>
