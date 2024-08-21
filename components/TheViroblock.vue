<template>
  <div class="container">
    <div class="photos">
      <div class="circle"></div>
      <img src="../public/viroblock1.svg" alt="" class="photo1" />
      <img src="../public/viroblock2.svg" alt="" class="photo2" />
    </div>
    <div class="texts">
      Enhanced with HeiQ Viroblock
      <span class="title">
        The UK’s First Fully Recyclable & Sustainable Face Mask
      </span>
      <span class="subtitle">
        At a time when the British public is required to wear a face mask when
        on trains, in shops and any enclosed space, 1TcA has launched the first
        British made reusable, sustainable face masks and snoods, manufactured
        using GRS fabric, woven from recycled waste plastic and treated.
      </span>
      <span class="learn"> Learn More -> </span>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.photo1 {
  width: 323px;
  height: 394px;
  position: absolute;
  top: 0;
  left: 35px;
}
.photo2 {
  width: 267px;
  height: 209px;
  position: absolute;
  bottom: 50px;
  right: 50px;
}
.container {
  width: 100%;
  max-width: 1270px;
  height: 520px;
  display: flex;
  flex-wrap: wrap;
  gap: 35px;
  position: relative;
  justify-content: space-evenly;
}
.photos {
  position: relative;
  max-width: 520px;
  height: 520px;
}
.circle {
  width: 520px;
  height: 520px;
  position: relative;
  top: -50px;
  left: 0;
  background-color: #006ff9;
  opacity: 0.1;
  border-radius: 100%;
}
.texts {
  width: 456px;
  height: 310px;
  position: relative;
  top: 50px;
  gap: 15px;
  text-transform: uppercase;
  color: #006ff9;
  font-size: 14px;
  display: flex;
  flex-direction: column;
  font-weight: 600;
  line-height: 18px;
  letter-spacing: 2px;
  text-align: left;
}
.title {
  font-size: 26px;
  font-weight: 600;
  line-height: 36px;
  text-transform: none;
  text-align: left;
  color: #212529;
}
.subtitle {
  font-size: 15px;
  font-weight: 400;
  text-transform: none;
  line-height: 28px;
  text-align: left;
  color: #6f7074;
}
.learn {
  font-size: 16px;
  font-weight: 500;
  line-height: 15px;
  text-align: left;
  text-transform: none;
  color: black;
  transition: all 0.5s ease;
  cursor: pointer;
  margin-bottom: 125px;
}
.learn:hover {
  translate: 5px 0px;
}
@media (min-width: 300px) {
  .circle {
    width: 320px;
    height: 320px;
  }
  .photos {
    display: flex;
    justify-content: center;
  }
  .photo1 {
    scale: 0.6;
    top: -110px;
    left: -20px;
  }
  .photo2 {
    scale: 0.6;
    bottom: 220px;
    right: -15px;
  }
  .texts {
    position: relative;
    width: 90%;
    top: -230px;
  }
}
@media (min-width: 600px) {
  .circle {
    width: 420px;
    height: 420px;
  }
  .photos {
    display: flex;
    justify-content: center;
  }
  .photo1 {
    scale: 0.7;
    top: -50px;
    left: 40px;
  }
  .photo2 {
    scale: 0.7;
    bottom: 140px;
    right: 15px;
  }
  .texts {
    position: relative;
    width: 90%;
    top: -120px;
  }
}
@media (min-width: 900px) {
  .circle {
    width: 420px;
    height: 420px;
  }
  .photos {
    display: flex;
    justify-content: center;
  }
  .photo1 {
    scale: 0.7;
    top: -50px;
    left: 40px;
  }
  .photo2 {
    scale: 0.7;
    bottom: 140px;
    right: 15px;
  }
  .texts {
    position: relative;
    top: 0px;
    width: 456px;
  }
}
@media (min-width: 1270px) {
  .circle {
    width: 520px;
    height: 520px;
  }
  .photo1 {
    scale: 1;
    top: 0;
    left: 35px;
  }
  .photo2 {
    scale: 1;
    bottom: 50px;
    right: 50px;
  }
  .texts {
    position: relative;
    top: 0px;
    width: 456px;
  }
}
</style>
