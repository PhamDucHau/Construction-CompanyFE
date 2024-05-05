<template>
  <div class="main">
    <div class="container">
      <div class="block-title">
        <h2>
          <span>Dự án của chúng tôi</span>
        </h2>
        <p>
          ND Contruction tự hào là đơn vị thi công các công trình nhà phố, biệt
          thự, căn hộ cao cấp, khách sạn - resort... Chúng tôi luôn nhận được sự
          hài lòng, tin tưởng hợp tác từ những khách hàng khó tính nhất.
        </p>
      </div>
      <v-card>
        <v-tabs v-model="tab" align-tabs="center" color="#ff5e14">
          <v-tab v-for="(item, index) in array" :key="index" :value="index">{{
            item.title
          }}</v-tab>
        </v-tabs>

        <v-tabs-window v-model="tab">
          <v-tabs-window-item v-for="n in 3" :key="n" :value="n">
            <v-container fluid class="content-tab">
              <v-row>
                <v-col
                  v-for="(item, index) in array[tab].child"
                  :key="index"
                  cols="12"
                  md="4"
                  class="item"
                >
                  <div class="item-blog">
                    <div class="block-thumb">
                      <a class="thumb" href="#">
                        <img :src="item.img" alt="" />
                      </a>
                    </div>
                    <div class="block-info">
                      <h3 v-text="item.title" />
                    </div>
                  </div>
                </v-col>
              </v-row>
            </v-container>
          </v-tabs-window-item>
        </v-tabs-window>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    tab: null,
    array: [
      {
        title: "Chung cư",
        child: [
          {
            title: "Căn hộ cao cấp 4 phòng ngủ - 220m2 - phong cách Luxury",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/duan-1.jpg?v=1681274377297",
          },
          {
            title: "Chung cư 120M2 – 3 phòng ngủ tại MHDI Lê Đức Thọ",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/duan-2.jpg?v=1681274550883",
          },
          {
            title: "Chung cư 105M2 – 3 phòng ngủ – phong cách hiện đại",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/duan-3.jpg?v=1681275227303",
          },
          {
            title: "Chưng cư 137M2 – 2 phòng ngủ – phong cách hiện đại",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/duan-4.jpg?v=1681282887083",
          },
          {
            title: "Chung cư 2 phòng ngủ – 96M2 – Phong cách INDOCHINE",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/duan-5.jpg?v=1681283162673",
          },
          {
            title: "Chung cư 2 phòng ngủ – 115M2 – Phong cách hiện đại",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/duan-6.jpg?v=1681283582287",
          },
        ],
      },
      {
        title: "Nhà đất",
        child: [
          {
            title: "Các loại thiết bị nhà bếp chuyên dùng cần thiết",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/t1.jpg?v=1681353123437",
          },
          {
            title:
              "Dự án nội thất phòng khách và tủ bếp tại Vinhomes Grand Park 3 PN",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/t2.jpg?v=1681353189973",
          },
          {
            title:
              "Nên sử dụng tủ bếp đóng sẵn hay tủ bếp thiết kế riêng cho gia đình",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/t3.jpg?v=1681353241560",
          },
          {
            title:
              "Tìm hiểu kính ốp tủ bếp là gì? Chọn mua kính ốp tủ bếp đẹp, chất lượng",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/t4.jpg?v=1681353311607",
          },
        ],
      },
      {
        title: "Biệt thự",
        child: [
          {
            title: "Các loại thiết bị nhà bếp chuyên dùng cần thiết",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/t1.jpg?v=1681353123437",
          },
          {
            title:
              "Dự án nội thất phòng khách và tủ bếp tại Vinhomes Grand Park 3 PN",
            img: "	https://bizweb.dktcdn.net/100/483/185/articles/t2.jpg?v=1681353189973",
          },
          {
            title:
              "Nên sử dụng tủ bếp đóng sẵn hay tủ bếp thiết kế riêng cho gia đình",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/t3.jpg?v=1681353241560",
          },
          {
            title:
              "Tìm hiểu kính ốp tủ bếp là gì? Chọn mua kính ốp tủ bếp đẹp, chất lượng",
            img: "https://bizweb.dktcdn.net/100/483/185/articles/t4.jpg?v=1681353311607",
          },
        ],
      },
    ],
  }),
};
</script>

<style scoped>
.main {
  position: relative;
  padding-top: 70px;
  overflow: hidden;
}
.main:before {
  content: "";
  background-image: url(//bizweb.dktcdn.net/100/483/185/themes/937690/assets/bg-project-tab.jpg?1705917002323);
  background-position: top left;
  background-repeat: no-repeat;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  width: 100%;
  height: 550px;
  background-attachment: fixed;
}
.container {
  max-width: 1140px;
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
}
.block-title {
  text-align: center;
  margin-bottom: 30px;
  color: #fff;
}
.block-title h2 {
  font-size: 40px;
  font-weight: 700;
}
.block-title p {
  font-size: 16px;
  margin: 0 180px;
}
.content-tab .item-blog {
  position: relative;
  box-shadow: 0px 6px 15px rgba(14, 18, 29, 0.06);
  margin-bottom: 30px;
  background: #fff;
}
.content-tab .item-blog .block-thumb .thumb {
  padding-bottom: 57%;
  display: block;
  height: 0;
  position: relative;
}
.content-tab .item-blog .block-thumb .thumb img {
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  max-width: 100%;
  max-height: 100%;
  width: auto !important;
  height: auto !important;
  position: absolute;
}
.content-tab .item-blog .block-info {
  padding: 15px 15px 20px;
  text-align: center;
}
.content-tab .item-blog .block-info h3 {
  font-size: 16px;
  min-height: 45px;
  margin-bottom: 0;
}
</style>