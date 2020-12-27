<template>
  <div class="container">
    <div id="fineDustMap" style="width:100vw; height:100vh"></div>
  </div>
</template>

<script>
export default {
  mounted() {
    const container = document.getElementById('fineDustMap')
    const options = {
      // 지도 생성시 기본 옵션
      center: new kakao.maps.LatLng(33.450701, 126.570667), // 지도 중심 좌표
      level: 3, // 지도레벨
    }

    const map = new kakao.maps.Map(container, options)
  },
}
</script>

<style>
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>