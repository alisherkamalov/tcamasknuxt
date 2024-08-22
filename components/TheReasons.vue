<template>
  <div class="container">
    <div class="texts">
      5 Reasons To Use 1TcA Masks
      <div class="cont-reasons" v-for="(reason, index) in reasons" :key="index"
      :style="{
        alignItems: reason.align
      }"
      >
        <img src="../public/checkmark.svg" alt="" class="check-mark" 
        :style="{
            marginTop: reason.top
        }"
        />
        <span class="reasons">
          {{ reason.text }}
        </span>
      </div>
    </div>
    <div class="photos">
        <img src="../public/reason-img.svg" alt="" class="reason-img" />
        <img src="../public/popb.svg" alt="" class="popb-img">
    </div>
    
  </div>
</template>

<script>
export default {
  setup() {
    const reasons = [
      {
        text: "Enhanced with HeiQ Viroblock",
        align: 'center',
        top: '0px'
      },
      {
        text: "Reduces cross contamination from hand to face covering",
        align: 'center',
        top: '0px'
      },
      {
        text: "Sustanable – protecting you and your planet",
        align: 'center',
        top: '0px'
      },
      {
        text: "British Manufacturing – helping the economy",
        align: 'center',
        top: '0px'
      },
      {
        text: "Cost-effective with all profits donated to our chosen charities",
        align: 'start',
        top: '5px'
      },
    ];
    return {
      reasons,
    };
  },
};
</script>

<style scoped>
.container {
  width: 100%;
  max-width: 1270px;
  height: 510px;
  display: flex;
  padding-bottom: 50px;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: center;
}
.reason-img {
  width: 451px;
  height: 510px;
}
.texts {
  width: 454px;
  font-size: 36px;
  font-weight: 600;
  gap: 15px;
  display: flex;
  flex-direction: column;
  line-height: 43.57px;
  text-align: left;
}
.cont-reasons {
  display: flex;
  gap: 10px;
}
.reasons {
  font-size: 16px;
  font-weight: 400;
  line-height: 26px;
  text-align: left;
  color: #6F7074;
}
.check-mark {
  width: 14px;
  height: 14px;
}
.photos {
    position: relative;
}
.popb-img {
    left: -75px;
    bottom: -75px;
    position: absolute;
}
@media(min-width:300px) {
    .texts {
        width: 90%;
        margin-top: 50px;
    }
    .reason-img {
        scale: 0.7;
        position: relative;
        left: -35px;
    }
    .popb-img {
        scale: 0.7;
        left: -15px;
        bottom: 0;
    }
    .photos {
        overflow: hidden;
    }
}
@media(min-width:600px) {
    .photos {
        overflow: visible;
    }
    .texts {
        width: 90%;
        margin-top: 50px;
        text-align: center;
        align-items: center;
    }
    .reason-img {
        scale: 0.9;
        position: relative;
        left: 0px;
    }
    .popb-img {
        scale: 0.9;
        left: -40px;
        bottom: -15px;
    }
}
@media(min-width:900px) {
    .photos {
        overflow: visible;
    }
    .texts {
        width: 90%;
        margin-top: 50px;
        text-align: center;
        align-items: center;
    }
    .reason-img {
        scale: 0.9;
        position: relative;
        left: 0;
    }
    .popb-img {
        scale:0.9;
        left: -35px;
        bottom: -15px;
    }
   
}
@media(min-width:1270px) {
    .photos {
        overflow: visible;
    }
    .texts {
        width: 454px;
        margin-top: 0px;
        text-align: left;
        align-items: start;
    }
    .reason-img {
        scale: 1;
        position: relative;
        left: 0;
    }
    .popb-img {
        scale:1;
        left: -75px;
        bottom: -75px;
    }
}
</style>
