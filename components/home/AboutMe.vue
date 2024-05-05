<template>
  <div class="main">
    <div class="container">
      <v-row>
        <v-col cols="6" class="block-title">
          <div class="about-text-1">Về chúng tôi</div>
          <h2>Chúng tôi dẫn đầu trong <br />lĩnh vực xây dựng</h2>
          <div class="about-text-2">
            Chất lượng – An toàn – Hiệu quả – Chuyên nghiệp
          </div>
          <div class="about-des">
            ND Construction là 1 trong những đơn vị đi đầu trong lĩnh vực thiết
            kế & thi công trọn gói. Trải qua nhiều năm hình thành và phát triển,
            chúng tôi vẫn giữ nguyên một sứ mệnh duy nhất: cung cấp dịch vụ thi
            công trọn gói các công trình dân dụng với những chiến lược thay đổi
            linh hoạt trong quá trình vận hành và phát triển.
          </div>
          <v-btn
            variant="outlined"
            size="large"
            style="background: #ff5e14; color: white"
            >Xem Thêm</v-btn
          >
        </v-col>
        <v-col cols="6" class="block-image">
          <img
            src="https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/about_banner_img.png?1705917028189"
            width="540"
            height="436"
            alt=""
          />
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main {
  display: flex;
  justify-content: center;
  margin-bottom: 70px;
}
.container {
  max-width: 1140px;
}
.block-title .about-text-1 {
  position: relative;
  display: inline-block;
  color: #ff5e14;
  font-size: 16px;
  text-transform: uppercase;
  letter-spacing: 0.2em;
}
.block-title h2 {
  font-size: 40px;
  line-height: initial;
  font-weight: 700;
  margin-top: 10px;
  position: relative;
  margin-bottom: 15px;
  padding-bottom: 15px;
}
.block-title h2:before {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 2px;
  width: 40px;
  content: "";
  background-color: #ff5e14;
}
.block-title .about-text-2 {
  font-size: 22px;
  color: #ff5e14;
  font-weight: 500;
  margin-bottom: 15px;
}
.block-title .about-des {
  font-size: 17px;
  line-height: 1.6;
  margin-bottom: 15px;
}
</style>