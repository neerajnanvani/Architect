<template>
  <div id="header_div">
    <v-img
      class="ma-auto pos-rel"
      :src="require('@/assets/architect.jpg')"
      max-width="1500px"
      max-height="800px"
    >
    </v-img>
    <div class="center_logo">
      <span id="span_first">BR</span>
      <span>Architects</span>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.pos-rel {
  position: relative;
  z-index: 0;
}
#header_div {
  position: relative;
}
.center_logo {
  position: absolute !important;
  font-weight: 400;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: 36px;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: white;
  z-index: 1;

  letter-spacing: 4px !important;
}
.center_logo #span_first {
  background-color: #000;
  color: white;
  padding: 8px 16px;
  font-weight: bold;
  opacity: 0.7;
  margin-right: 14px;
}

</style>