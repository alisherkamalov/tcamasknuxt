<template>
  <div class="container">
    <div class="cont" v-for="(container, index) in containers" :key="index">
      <img :src="container.image" alt="" class="protect-img" />
      {{ container.title }}
      <span class="subtitle">
        {{ container.subtitle }}
      </span>
      <button class="shop-now">Shop Now</button>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    const containers = [
      {
        image: "../protect-img1.svg",
        title: "Protect your family",
        subtitle: "Purchase our family packs of masks online",
      },
      {
        image: "../protect-img2.svg",
        title: "Protect The Public",
        subtitle: "Purchase our family packs of masks online",
      },
      {
        image: "../protect-img3.svg",
        title: "Protect Your Employess",
        subtitle: "Purchase our family packs of masks online",
      },
    ];
    return {
      containers,
    };
  },
};
</script>

<style scoped>
.subtitle {
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  text-align: center;
  color: #6f7074;
}
.container {
  width: 100%;
  max-width: 1270px;
  padding-top: 90px;
  padding-bottom: 90px;
  height: auto;
  gap: 25px;
  background-color: #f4f9fe;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
.shop-now {
  width: 120px;
  height: 38px;
  background-color: #006ff9;
  color: white;
  border-radius: 4px;
  font-size: 15px;
  font-weight: 500;
  line-height: 24px;
  text-align: center;
  cursor: pointer;
  border: 0;
  transition: all 0.2s ease;
}
.cont {
  width: 350px;
  height: 533px;
  position: relative;
  display: flex;
  font-size: 26px;
  font-weight: 600;
  align-items: center;
  line-height: 22px;
  text-align: center;
  flex-direction: column;
  gap: 15px;
}
.protect-img {
  width: 350px;
  height: 370px;
}
</style>
