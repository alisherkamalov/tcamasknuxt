<template>
  <div class="container">
    <div class="donated">
      <div class="cube-one"></div>
      <div class="cube-two"></div>
      <span class="title">
        All 1TCA profits are donated to charitable Causes and community projects
      </span>
      <button class="shop-now">Shop Now -></button>
    </div>
    <div class="bottom-footer">
      <img src="../public/img-footer.svg" alt="" class="bg-img-footer" />
      <div class="content">
        <div class="logo-texts">
          <img src="../public/white-logo.svg" alt="" class="logo" />
          Textiles are one of the main vectors for viruses and bacteria.
          Textiles treat with HeiQ viroblock.
          <div class="icons">
            <svg
              class="f-ico"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 320 512"
            >
              <!--!Font Awesome Free 6.6.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
              <path
                fill="#6f7074"
                d="M80 299.3V512H196V299.3h86.5l18-97.8H196V166.9c0-51.7 20.3-71.5 72.7-71.5c16.3 0 29.4 .4 37 1.2V7.9C291.4 4 256.4 0 236.2 0C129.3 0 80 50.5 80 159.4v42.1H14v97.8H80z"
              />
            </svg>
            <svg
              class="y-ico"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 576 512"
            >
              <!--!Font Awesome Free 6.6.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
              <path
                fill="#6f7074"
                d="M549.7 124.1c-6.3-23.7-24.8-42.3-48.3-48.6C458.8 64 288 64 288 64S117.2 64 74.6 75.5c-23.5 6.3-42 24.9-48.3 48.6-11.4 42.9-11.4 132.3-11.4 132.3s0 89.4 11.4 132.3c6.3 23.7 24.8 41.5 48.3 47.8C117.2 448 288 448 288 448s170.8 0 213.4-11.5c23.5-6.3 42-24.2 48.3-47.8 11.4-42.9 11.4-132.3 11.4-132.3s0-89.4-11.4-132.3zm-317.5 213.5V175.2l142.7 81.2-142.7 81.2z"
              />
            </svg>
            <svg
              class="l-ico"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 448 512"
            >
              <!--!Font Awesome Free 6.6.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
              <path
                fill="#6f7074"
                d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3zM135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5 0 21.3-17.2 38.5-38.5 38.5zm282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5 67.2 0 79.7 44.3 79.7 101.9V416z"
              />
            </svg>
            <svg
              class="i-ico"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 448 512"
            >
              <!--!Font Awesome Free 6.6.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.-->
              <path
                fill="#6f7074"
                d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z"
              />
            </svg>
          </div>
        </div>
        <div class="navigation">
          Navigation
          <div class="line"></div>
          <ul class="ul-nav">
            <li>Shop</li>
            <li>About Us</li>
            <li>Contact Us</li>
            <li>Privacy Policy</li>
            <li>Cart</li>
            <li>Terms And Conditions</li>
            <li>Recyclable</li>
          </ul>
        </div>
        <div class="company">
          Company Details
          <div class="line"></div>
          <ul class="ul-company">
            <li>
              <img src="../public/phone-ico.svg" alt="" class="li-ico" />
              <span class="info">020 7520 9260</span>
            </li>
            <li>
              <img src="../public/email-ico.svg" alt="" class="li-ico" />
              <span class="info">Contact@1tca.com</span>
            </li>
            <li>
              <img src="../public/location-ico.svg" alt="" class="li-ico" />
              <span class="info"
                >Adam House, 7 – 10 Adams Street, The Strand, London WC2N
                6AA</span
              >
            </li>
          </ul>
        </div>
        <div class="partner">
          Our Partner
          <div class="line"></div>
          <ul class="ul-partner">
            <li>HeiQ</li>
            <li>Project Plan B</li>
            <li><img src="../public/popb.svg" alt="" class="img-partner" /></li>
          </ul>
        </div>
      </div>
      <div class="privacy">
        <div class="line-bottom"></div>
        ©2020 1TCA | PRIVACY POLICY | Disclaimer
      </div>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.privacy {
  display: flex;
  width: 100%;
  flex-direction: column;
  gap: 25px;
  align-items: center;
  color: #6f7074;
  font-size: 14px;
  font-weight: 400;
  line-height: 30px;
  text-align: left;
}
.content {
  display: flex;
  gap: 70px;
  position: relative;
  top: 120px;
  justify-content: center;
  flex-wrap: wrap;
}
.ul-company {
  gap: 5px;
  display: flex;
  flex-direction: column;
}
.line-bottom {
  width: 80%;
  height: 0px;
  padding-top: 0.5px;
  padding-bottom: 0.5px;
  background-color: #6f7074;
}
.ul-partner {
  display: flex;
  flex-direction: column;
  gap: 5px;
  font-size: 14px;
  font-weight: 400;
  line-height: 30px;
  text-align: left;
}
.img-partner {
  width: 120px;
  height: 120px;
}
.partner {
  width: 160px;
  height: 260px;
  font-size: 16px;
  font-weight: 500;
  line-height: 21px;
  text-align: left;
  color: #d3d3d4;
  display: flex;
  flex-direction: column;
  gap: 15px;
}
.bg-img-footer {
  width: 865.29px;
  height: 524px;
  object-fit: contain;
  position: absolute;
  bottom: 0;
  right: 0;
}
.company {
  font-size: 16px;
  font-weight: 500;
  line-height: 21px;
  width: 100%;
  gap: 15px;
  display: flex;
  flex-direction: column;
  color: #d3d3d4;
  max-width: 255px;
  height: 260px;
  text-align: left;
}
.li-ico {
  width: 13.97px;
  height: 14px;
  margin-right: 5px;
  position: relative;
  top: 1px;
}
.info {
  font-size: 14px;
  font-weight: 300;
  line-height: 14px;
  text-align: left;
  color: #d3d3d4;
}
.ul-nav {
  font-size: 14px;
  font-weight: 400;
  line-height: 30px;
  text-align: left;
  padding: 0;
  margin: 0;
  list-style: none;
}

.ul-nav li {
  margin: 0;
  padding: 0;
}

.line {
  width: 100%;
  height: 0px;
  padding-top: 0.5px;
  padding-bottom: 0.5px;
  background-color: #6f7074;
}
.navigation {
  width: 161px;
  height: 260px;
  display: flex;
  gap: 15px;
  flex-direction: column;
  font-size: 16px;
  font-weight: 500;
  line-height: 21px;
  text-align: left;
  color: #d3d3d4;
}
.logo {
  width: 68.94px;
  height: 40px;
}
.icons {
  display: flex;
  width: 144px;
  height: 24px;
  position: relative;
  left: -10px;
}
.logo-texts {
  display: flex;
  flex-direction: column;
  gap: 20px;
  font-size: 14px;
  width: 242px;
  height: 260px;
  font-weight: 400;
  line-height: 22px;
  text-align: left;
  color: #d3d3d4;
}
.shop-now {
  width: 200px;
  height: 56px;
  border: 0;
  color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
  font-weight: 500;
  line-height: 30px;
  letter-spacing: 0.04em;
  text-align: left;
  transition: all 0.5s ease;
  background-color: white;
  border-radius: 2px;
}
.container {
  width: 100%;
  height: 836.5px;
  display: flex;
  position: relative;
  justify-content: center;
}
.bottom-footer {
  width: 100%;
  height: 673px;
  position: absolute;
  bottom: 0;
  justify-content: center;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  background-color: #212529;
}
.donated {
  width: 90%;
  max-width: 1110px;
  height: 327px;
  position: relative;
  display: flex;
  z-index: 1;
  overflow: hidden;
  gap: 25px;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  border-radius: 10px;
  background-color: #006ff9;
}
.title {
  color: white;
  font-size: 36px;
  font-weight: 600;
  line-height: 44px;
  text-align: center;
  width: 100%;
  max-width: 878px;
}
.cube-one {
  width: 188.61px;
  height: 226.91px;
  background-color: #ffffff;
  border-radius: 37px;
  opacity: 0.1;
  position: absolute;
  left: -25px;
  bottom: -25px;
  rotate: 46.95deg;
}
.cube-two {
  width: 188.61px;
  height: 226.91px;
  background-color: #ffffff;
  border-radius: 37px;
  opacity: 0.1;
  right: -25px;
  top: -25px;
  position: absolute;
  rotate: -127.98deg;
}
@media (min-width: 300px) {
    .title {
        width: 90%;
        font-size: 26px;
    }
    .bottom-footer {
        height: 1573px;
        
    }
    .company {
        height: 150px;
    }
    .logo-texts {
        height: 200px;
    }
    .container {
        height: 1800px;
    }
}
@media (min-width: 520px) {
    .title {
        width: 90%;
        font-size: 26px;
    }
    .bottom-footer {
        height: 1073px;
        
    }
    .company {
        height: 150px;
    }
    .logo-texts {
        height: 200px;
    }
    .container {
        height: 1300px;
    }
}
@media (min-width: 600px) {
    .title {
        width: 90%;
        font-size: 26px;
    }
    .bottom-footer {
        height: 873px;
        
    }
    .company {
        height: 260px;
    }
    .logo-texts {
        height: 260px;
    }
    .container {
        height: 1100px;
    }
}
@media (min-width: 900px) {
    .title {
        width: 90%;
        font-size: 26px;
    }
    .bottom-footer {
        height: 873px;
        
    }
    .company {
        height: 260px;
    }
    .logo-texts {
        height: 260px;
    }
    .container {
        height: 1100px;
    }
}
@media (min-width: 1270px) {
    .title {
        width: 90%;
        font-size: 36px;
    }
    .company {
        height: 260px;
    }
    .logo-texts {
        height: 260px;
    }
    .container {
        height: 836.5px;
    }
    .bottom-footer {
        height: 673px;
        padding-top: 0px;
        padding-bottom: 0px;
    }
}
</style>
