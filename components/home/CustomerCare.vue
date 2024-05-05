<template>
  <div class="main">
    <div class="container">
      <v-row>
        <v-col
          cols="3"
          v-for="(item, index) in array"
          :key="index"
          class="item"
        >
          <div class="inner">
            <div class="img-title">
              <div class="image mb-5">
                <img class="d-flex" :src="item.img" alt="" />
              </div>
              <h3 class="mb-2 text-justify" v-text="item.title" />
            </div>
            <div class="contentsv text-justify" v-text="item.description" />
          </div>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      array: [
        {
          img: "https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/ico_policy1.png?1705917028189",
          title: "Cam kết chất lượng",
          description:
            "Chất lượng luôn được ưu tiên trong từng hạng mục, chi tiết nhỏ nhất mang đến sự yên tâm cho khách hàng.",
        },
        {
          img: "https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/ico_policy2.png?1705917028189",
          title: "Đảm bảo đúng thời gian",
          description:
            "Cam kết đúng thời gian, tiến độ đã trở thành truyền thống phong cách làm việc của QD Construction.",
        },
        {
          img: "https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/ico_policy3.png?1705917028189",
          title: "Tận tâm với khách hàng",
          description:
            "Phục vụ khách hàng chu đáo như “thượng đế” trở thành kim chỉ nam hàng đầu cho mọi hành động.",
        },
        {
          img: "https://bizweb.dktcdn.net/100/483/185/themes/937690/assets/ico_policy4.png?1705917028189",
          title: "Bảo hành dài hạn",
          description:
            "Chính sách bảo hành dài hạn như để khẳng định giá trị cốt lõi, thương hiệu mà Roman luôn hướng tới.",
        },
      ],
    };
  },
};
</script>

<style scoped>
.main {
  display: flex;
  justify-content: center;
  margin-bottom: 70px;
}
.container {
  max-width: 1140px;
  text-align: center;
}

.item .img-title .image img {
  -webkit-transition: 0.4s ease-in-out;
  transition: 0.4s ease-in-out;
}
.item:hover .image img {
  -webkit-transform: rotateY(180deg);
  transform: rotateY(180deg);
}
.inner {
  background-color: #fff;
  border-top: 5px solid #ff5e14;
  box-shadow: 0px 6px 15px rgba(14, 18, 29, 0.06);
  border-radius: 10px;
  padding: 25px;
}
</style>