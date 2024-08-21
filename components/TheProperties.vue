<template>
  <div class="container">
    The Unique properties of our 1TCA mask
    <span class="title">
      British public is required to wear a face mask when on trains, in shops
      and any enclosed space, 1TcA has launched the first.
    </span>
    <div class="containers">
      <div
        :class="container.class"
        v-for="(container, index) in containers"
        :key="index"
        :style="{
          backgroundColor: container.color,
          border: container.border,
          color: container.color_text,
        }"
      >
        <div
          class="icon-cont"
          :style="{
            backgroundColor: container.i_c_color,
          }"
        >
          <img :src="container.image" alt="effective ico" class="e-ico" />
        </div>
        {{ container.title }}
        <span
          class="subtitle"
          :style="{
            color: container.color_subtitle,
          }"
        >
          {{ container.subtitle }}
        </span>
        <span
          class="learn"
          :style="{
            color: container.l_m_color,
          }"
        >
          Learn More ->
        </span>
      </div>
      <img
        src="../public/yellow-right.svg"
        alt="yellow right"
        class="yellow-right"
      />
    </div>
  </div>
</template>

<script lang="ts">
export default {
  setup() {
    const containers = [
      {
        class: "cont one",
        image: "../effective-ico.svg",
        i_c_color: "#006FF9",
        color: "white",
        border: "1px solid #E9E9EA",
        title: "Effective",
        color_text: "black",
        color_subtitle: "gray",
        subtitle:
          "HeiQ viroblock works to deactivate. the virus with minutes and effective for 30 washes.",
        l_m_color: "black",
      },
      {
        class: "cont two",
        image: "../recyclable-ico.svg",
        i_c_color: "white",
        color: "#006FF9",
        border: "0",
        l_m_color: "white",
        title: "Recyclable",
        color_text: "white",
        color_subtitle: "#FAFAFA",
        subtitle:
          "HeiQ viroblock works to deactivate. the virus with minutes and effective for 30 washes.",
      },
      {
        class: "cont three",
        image: "../practical-ico.svg",
        i_c_color: "#006FF9",
        color: "white",
        border: "1px solid #E9E9EA",
        l_m_color: "black",
        title: "Practical",
        color_subtitle: "gray",
        color_text: "black",
        subtitle:
          "HeiQ viroblock works to deactivate. the virus with minutes and effective for 30 washes.",
      },
    ];

    return {
      containers,
    };
  },
};
</script>

<style scoped>
.learn {
  font-size: 16px;
  font-weight: 500;
  line-height: 15px;
  text-align: left;
  transition: all 0.5s ease;
}
.learn:hover {
  translate: 5px 0px;
}
.subtitle {
  width: 298px;
  font-size: 15px;
  font-weight: 400;
  line-height: 28px;
  text-align: left;
}
.icon-cont {
  width: 62px;
  height: 62px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 8px;
}
.yellow-right {
  width: 323.15px;
  height: 749px;
  position: absolute;
  right: 0;
  top: 200px;
}
.container {
  width: 100%;
  max-width: 1270px;
  height: 630px;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  font-size: 36px;
  padding-top: 70px;
  font-weight: 600;
  gap: 15px;
  line-height: 43.57px;
  text-align: center;
}
.cont {
  width: 314px;
  padding: 20px;
  height: 314px;
  z-index: 1;
  display: flex;
  flex-direction: column;
  gap: 25px;
  border-radius: 10px;
  font-size: 22px;
  font-weight: 500;
  line-height: 22px;
  text-align: left;
  transition: all 0.5s ease;
}
.cont.one:hover {
  translate: 0px -10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.cont.two:hover {
  translate: 0px -10px;
  box-shadow: #006ff9 0px 7px 29px 0px;
}
.cont.three:hover {
  translate: 0px -10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.title {
  font-size: 15px;
  font-weight: 400;
  line-height: 26px;
  text-align: center;
  color: #999999;
  width: 572px;
}
.containers {
  width: 100%;
  max-width: 1270px;
  display: flex;
  gap: 15px;
  margin-top: 25px;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
@media (min-width: 300px) {
  .container {
    font-size:20px;
  }
  .title {
    width: 90%;
  }
  .cont {
    width: 80%;
  }
  .containers {
    width: 90%;
  }
}
@media (min-width: 600px) {
  .cont {
    width: 314px;
  }
}
@media (min-width: 900px) {
  .cont {
    width: 314px;
  }
}
@media (min-width: 1270px) {
  .cont {
    width: 314px;
  }
}
</style>
