<template>
  <div class="container">
    What our client say about us
    <span class="title">
      British public is required to wear a face mask when on trains, in shops
      and any enclosed space, 1TcA has launched the first.
    </span>
    <div class="reviews">
      <div class="flex-review">
        <div
          class="column-review"
          v-for="(review, index) in reviews"
          :key="index"
        >
          <div class="review">
            <div class="center-ico">
              <div class="about-ico-cont">
                <img
                  src="../public/about-ico.svg"
                  alt="about ico"
                  class="about-ico"
                />
              </div>
            </div>

            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Auctor
            neque sed imperdiet nibh lectus feugiat nunc sem. when an unknown
            printer took a galley.
          </div>
          <div class="center-triagle">
            <div class="triagle"></div>
          </div>
          
          <div class="flex-users">
            <div class="info-user">
              <img :src="review.img" alt="" class="avatar" />
              {{ review.name }}
              <span class="user-title">{{ review.title }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    const reviews = [
      {
        img: "../avatar-about.svg",
        name: "Jane Cooper",
        title: "CEO at Design Space",
      },
      {
        img: "../avatar-about.svg",
        name: "Jane Cooper",
        title: "CTO at Google Maps",
      },
      {
        img: "../avatar-about.svg",
        name: "Jane Cooper",
        title: "CEO at ABC Corporation",
      },
    ];

    return {
      reviews,
    };
  },
};
</script>

<style scoped>
.flex-users {
  min-width: 100%;
  display: flex;
  flex-shrink: 0;
  gap: 15px;
}
.triagle {
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
  width: 24px;
  height: 15.5px;
  rotate: 180deg;
  background-color: white;
}
.center-triagle {
    min-width: 290px;
    display: flex;
    justify-content: center;
}
.user-title {
  font-size: 14px;
  font-weight: 400;
  line-height: 24px;
  text-align: center;
  color: #6f7074;
}
.avatar {
  width: 56px;
  height: 56px;
  margin-bottom: 10px;
}
.info-user {
  width: 100%;

  height: 200px;
  display: flex;
  font-size: 18px;
  font-weight: 500;
  line-height: 28px;
  text-align: center;

  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.about-ico-cont {
  width: 54px;
  height: 54px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 100%;
}
.center-ico {
  width: 81%;
  height: auto;
  display: flex;
  justify-content: center;
  position: absolute;
  top: -10px;
}
.about-ico {
  width: 35.34px;
  height: 30px;
}
.container {
  width: 100%;
  max-width: 1270px;
  display: flex;
  overflow-x: hidden;
  flex-direction: column;
  align-items: center;
  font-size: 36px;
  margin-bottom: 150px;
  font-weight: 500;
  line-height: 43.57px;
  gap: 15px;
  text-align: center;
  margin-top: 70px;
}
.reviews {
  max-width: 1110px;
  width: 100%;
  gap: 15px;
  margin-top: 50px;
  height: auto;
  display: flex;
  flex-shrink: 0;
  align-items: center;
  flex-direction: column;
  overflow-x: auto;
  justify-content: flex-start;
  scroll-behavior: smooth;
  padding-left: 15px;
  padding-right: 15px;
}

.flex-review {
  display: flex;
  flex-shrink: 0;
  gap: 15px;
  justify-content: center;
  width: 100%;
}

.column-review {
  display: flex;
  width: 290px;
  flex-direction: column;
  flex-shrink: 0;
}

.review {
  position: relative;
  max-width: 290px;
  padding-left: 30px;
  padding-right: 30px;
  height: auto;
  flex-shrink: 0;
  padding-top: 48px;
  padding-bottom: 48px;
  box-shadow: 0px 30px 40px 0px #d4d9e833;
  border-radius: 10px;
  display: flex;
  justify-self: center;
  flex-shrink: 0;
  align-items: center;
  font-size: 14px;
  font-weight: 400;
  line-height: 24px;
  text-align: center;
}

.title {
  font-size: 15px;
  font-weight: 400;
  line-height: 26px;
  text-align: center;
  color: #999999;
  width: 572px;
}

@media (min-width: 300px) {
  .flex-review {
    justify-content: start;
    padding-left: 25px;
    padding-right: 25px;
  }
  .title {
    width: 90%;
  }
}
@media (min-width: 600px) {
  .flex-review {
    justify-content: start;
    padding-left: 25px;
    padding-right: 25px;
  }
  .title {
    width: 90%;
  }
}
@media (min-width: 900px) {
  .flex-review {
    justify-content: center;
    padding-left: 0px;
    padding-right: 0px;
  }
  .title {
    width: 572px;
  }
}
@media (min-width: 1270px) {
  .flex-review {
    justify-content: center;
    padding-left: 0px;
    padding-right: 0px;
  }
  .title {
    width: 572px;
  }
}
</style>
