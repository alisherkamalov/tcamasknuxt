<template>
  <nav>
    <div class="container">
      <img src="/logo.svg" alt="logo" class="logo" />
      <button class="burger-btn" @click="BurgerMenu">
        <div class="lines">
          <div class="line" v-for="(line, index) in lines" :key="index"></div>
        </div>
      </button>
      <ul class="ul-nav">
        <li class="li-home">Home</li>
        <li class="li-about">About</li>
        <li class="li-secience">The Secience</li>
        <li class="li-bulk">Shop Bulk</li>
        <li class="li-ordering">Ordering</li>
        <li class="li-news">News</li>
      </ul>
      <div class="buttons">
        <button class="cart">
          <img src="/cart.svg" alt="cart" class="cart-ico" />
        </button>
        <button class="contact">Contact</button>
      </div>
    </div>
  </nav>
  <div class="burger-menu" :style="{ display: dispmenu }">
    <div
      class="black-bg"
      :style="{ opacity: blackbg }"
      @click="BurgerMenu"
    ></div>
    <div
      class="content-menu"
      :style="{ transform: `translate(${offsetmenu})` }"
    >
      <img src="/logo.svg" alt="logo" class="logo-mob" />
      <ul class="ul-nav-mob">
        <li class="li-home">Home</li>
        <li class="li-about">About</li>
        <li class="li-secience">The Secience</li>
        <li class="li-bulk">Shop Bulk</li>
        <li class="li-ordering">Ordering</li>
        <li class="li-news">News</li>
      </ul>
    </div>
  </div>
</template>

<script>
import { ref, onMounted } from "vue";
export default {
  setup() {
    const lines = [{}, {}, {}];
    const isOpen = ref(false);
    const blackbg = ref(0);
    const dispmenu = ref("none");
    const offsetmenu = ref("-500px, 0px");

    const BurgerMenu = () => {
     

      isOpen.value = !isOpen.value;
      if (isOpen.value) {
        dispmenu.value = "flex";
        
        setTimeout(() => {
          offsetmenu.value = "0px, 0px";
          blackbg.value = 0.5;
        }, 10);
      } else {
        offsetmenu.value = "-500px, 0px";
        blackbg.value = 0;
        setTimeout(() => {
          dispmenu.value = "none";
          
        }, 500);
      }
    };

    onMounted(() => {
      
    });

    return {
      lines,
      
      isOpen,
      blackbg,
      offsetmenu,
      BurgerMenu,
      dispmenu,
    };
  },
};
</script>

<style scoped>
.burger-menu {
  width: 100%;
  height: 100%;
  position: absolute;
  display: none;
}
.black-bg {
  width: 100%;
  height: 100%;
  background-color: black;
  position: fixed;
  right: 0;
  top: 0;
  z-index: 99;
  transition: all 0.5s ease;
}
.content-menu {
  width: 200px;
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  z-index: 101;
  background-color: white;
  transition: all 0.5s ease;
}
.line {
  width: 25px;
  height: 1.5px;

  background-color: black;
  border-radius: 5px;
  transition: all 0.5s ease;
}
.lines {
  display: flex;
  flex-direction: column;
  gap: 7px;
  margin-bottom: 25px;
  transition: all 0.5s ease;
}
.burger-btn {
  border: 0;
  display: none;
  padding-left: 12px;
  padding-top: 11px;
  border-radius: 5px;
  border: 1px solid grey;
  padding-right: 12px;
  height: 42px;
  background-color: white;
  position: absolute;
  left: 25px;
  transition: all 0.5s ease;
}
.burger-btn:active {
  scale: 0.9;
}
.burger-btn:hover {
  background-color: #006ff9;
}
.lines:hover > .line {
  background-color: white;
}

.container {
  width: 100%;
  max-width: 1240px;
  display: flex;
  z-index: 4;
  overflow: hidden;
  justify-content: space-evenly;
}
.li-home,
.li-about,
.li-secience,
.li-bulk,
.li-ordering,
.li-news {
  transition: all 0.5s ease;
  cursor: pointer;
}
.li-home:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.li-about:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.li-secience:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.li-bulk:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.li-ordering:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.li-news:hover {
  color: #006ff9;
  translate: 0px -5px;
}
.buttons {
  display: flex;
  gap: 25px;
  position: relative;
  top: 2px;
}
.contact {
  width: 108px;
  height: 38px;
  background-color: white;
  border-radius: 4px;
  border: 0;
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
  text-align: center;
  cursor: pointer;
  transition: all 0.5s ease;
}
.contact:hover {
  background-color: #006ff9;
  color: white;
}
.cart-ico {
  width: 18px;
  height: 15.65px;
  position: relative;
  left: -1px;
  top: 1px;
}
.cart {
  width: 38px;
  height: 38px;
  border: 1px solid #006ff9;
  background-color: white;
  border-radius: 100%;
  cursor: pointer;
  transition: all 0.5s ease;
}
.cart:active {
  scale: 0.9;
}
.logo {
  width: 81.82px;
  height: 48px;
  margin-right: 25px;
}
.ul-nav {
  position: relative;
  left: -70px;
  height: 47px;
  display: flex;
  gap: 25px;
  background-color: white;
  padding-right: 33.5px;
  align-items: center;
  font-size: 15px;
  font-weight: 500;
  line-height: 20px;
  text-align: left;
}
.logo-mob {
  width: 81.82px;
  height: 48px;
  position: relative;
  top: 20px;
  left: 25px;
  margin-right: 25px;
}
.ul-nav-mob {
  position: relative;
  left: -70px;
  height: 47px;
  width: 100px;
  display: flex;
  flex-direction: column;
  gap: 25px;
  background-color: white;
  padding-right: 33.5px;
  align-items: left;
  font-size: 15px;
  font-weight: 500;
  left: 30px;
  top: 50px;
  line-height: 20px;
  text-align: left;
}
@media (min-width: 300px) {
    nav {
        width: 99.5%;
    }
  .buttons {
    position: relative;
    z-index: 4;
    margin-right: 25px;
  }
  .ul-nav {
    display: none;
  }
  .logo {
    display: none;
  }
  .burger-btn {
    display: flex;
    margin-left: 9px;
  }
  .container {
    justify-content: flex-end;
    align-items: center;
    height: 75px;
  }
}
@media (min-width: 600px) {
    nav {
        width: 99.5%;
    }
  .logo {
    display: none;
  }
  .ul-nav {
    display: none;
  }
  .burger-btn {
    display: flex;
  }
  .container {
    justify-content: flex-end;
    height: 75px;
  }
}
@media (min-width: 900px) {
    nav {
        width: 100%;
    }
  .buttons {
    z-index: 4;
  }
  .logo {
    display: none;
  }
  .ul-nav {
    display: none;
  }
  .burger-btn {
    display: flex;
  }
  .container {
    justify-content: flex-end;
    height: 75px;
  }
}
@media (min-width: 1270px) {
    nav {
        width: 100%;
    }
  .buttons {
    position: relative;
    z-index: 4;
  }
  .logo {
    display: flex;
  }
  .ul-nav {
    display: flex;
  }
  .burger-btn {
    display: none;
  }
  .container {
    justify-content: space-evenly;
    height: auto;
  }
}
</style>
