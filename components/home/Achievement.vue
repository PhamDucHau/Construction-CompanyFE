<template>
  <div class="main">
    <div class="container">
      <v-row>
        <v-col cols="6" class="col-left">
          <div class="title">
            <p>Thành tựu!</p>
            <h2>Thành tựu của chúng tôi</h2>
          </div>
          <div class="des">
            Với +18 năm trong nghề, ND Contruction luôn tự hào là đơn vị thiết
            kế thi công chuyên nghiệp, luôn mang lại giá trị thiết thực nhất tới
            khách hàng.
          </div>
          <v-row class="block-content">
            <v-col v-for="(item, index) in 4" :key="index" class="item">
              <div class="inner">
                <div class="icon">
                  <img
                    width="50"
                    height="50"
                    src="https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/why_choose_1.png?1705917028189"
                    alt=""
                  />
                </div>
                <div class="content">
                  <h3>18000</h3>
                  <p>Khách hàng</p>
                </div>
              </div>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="6" class="col-right">
          <div class="relative">
            <img
              width="540"
              height="383"
              src="https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/img_why_choose.jpg?1705917028189"
              alt=""
              style="border-radius: 4px"
            />
          </div>
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
  padding: 60px 0 60px;
  position: relative;
}
.container {
  max-width: 1140px;
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
}
.col-left .title p {
  position: relative;
  display: inline-block;
  color: #ff5e14;
  font-size: 16px;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  margin-bottom: 5px;
}
.col-left .title h2 {
  font-size: 40px;
  font-weight: 700;
}
.col-left .des {
  font-size: 16px;
  margin-bottom: 20px;
}
.block-content .item .inner {
  background: #fff;
  border-radius: 10px;
  display: flex;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.09);
  padding-left: 25px;
  padding-right: 25px;
  padding-bottom: 10px;
  align-items: center;
}
.block-content .item .inner .icon {
  width: 70px;
  background: #ff5e14;
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  padding: 10px 10px 25px;
}
.block-content .item .inner .content {
  width: calc(100% - 70px);
  padding-left: 20px;
  line-height: initial;
}
.block-content .item .inner .content h3 {
  font-size: 24px;
  color: #ff5e14;
  font-weight: bold;
  margin-bottom: 0;
}
.block-content .item .inner .content p {
  font-size: 16px;
  margin-bottom: 0;
}
.relative {
  position: relative;
}
</style>

