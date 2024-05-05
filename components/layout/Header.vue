<template>
  <header class="header">
    <v-row no-gutters class="d-flex">
      <v-col cols="5" class="col-main">
        <img
          class="logoHeader"
          style="border-radius: 8px"
          src="~/assets/img/logoHeader.png"
          alt="Discover Nuxt 3"
        />
      </v-col>
      <v-col cols="5" class="col-main">
        <ul class="d-flex">
          <li>TRANG CHỦ</li>
          <li>GIỚI THIỆU</li>
          <li>DỰ ÁN TIÊU BIỂU</li>
          <li>SẢN PHẨM</li>
          <li>ĐỘI NGŨ</li>
        </ul>
      </v-col>
    </v-row>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
.header {
  background-color: #050f2d;
  height: 100px;
  display: flex;
  text-align: center;
  align-items: center;
}
.header v-row {
}
.col-main {
  display: flex;
  justify-content: center;
  color: white;
}
ul {
  justify-content: space-between;
  list-style: none;
  width: 100%;
  align-items: center;
}
.logoHeader {
  height: 5rem;
}
</style>>


