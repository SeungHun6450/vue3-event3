<template>
<!-- 
  @keydown.key : key에는 케밥케이스로 작성하여 사용
  체이닝으로 사용이 가능하다
  ex) @keydoun.ctrl.shift.a="handler" -> ctrl,shift, a를 눌러야 반응
  ex) key에 a를 해놓으면 a를 눌러야 반응이 나옴
 -->
  <input
    type="text"
    @keydown.ctrl.a="handler" />
</template>

<script>
export default {
  methods: {
    handler(event) {
      // 엔터 사용 시 로그 띄우기
      // if (event.key === 'Enter') {
        console.log('Enter!!')
      // }
    }
  }
}
</script>