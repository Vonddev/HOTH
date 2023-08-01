<script setup>
const pdfPath = `${process.env.NODE_ENV == 'development' ? '/HoTH.pdf' : '/HOTH/HoTH.pdf'}`;
</script>

<template>
  <div class="frame">
    <embed class="pdfFrame" type="application/pdf" :src="pdfPath" width="100%" height="100%" />
  </div>
</template>

<style scoped>
.frame {
  height: 100vh;
}
.pdfFrame {
  border: none;
}
</style>
