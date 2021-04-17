<template>
  <div id="app">
      
      <div class="hContainer">
        <header class="header">
        
          <div class="header_logo">
            <router-link to="/">
              <img src="@/assets/img/logo.png" alt="">
            </router-link>
          </div>
          
          <ul class="header_links">
            <li class="header_links_link">
              <router-link to="/projects"> ПРОЕКТЫ </router-link>
            </li>
            <li class="header_links_link">
              <router-link to="/services"> УСЛУГИ </router-link>
            </li>
            <li class="header_links_link">
              <router-link to="/projects"> О НАС </router-link>
            </li>
            <li class="header_links_link">
              <router-link to="/projects"> КОНТАКТЫ </router-link>
            </li>
          </ul>

          <div class="header_lang">
            <button class="header_lang_btn"> RU </button>
            <button class="header_lang_btn"> EN </button>
          </div>
        </header>
      </div>
    
    <div class="container"> 
      <router-view/>
    </div>
      

  </div>
</template>

<style lang="scss" >
body, *{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

@font-face{
  font-family: 'rale-r';
  src: url('./assets/fonts/Raleway-Regular.ttf')
}
@font-face{
  font-family: 'rale-b';
  src: url('./assets/fonts/Raleway-Bold.ttf')
}
@font-face{
  font-family: 'rale-eb';
  src: url('./assets/fonts/Raleway-ExtraBold.ttf')
}
@font-face{
  font-family: 'rale-sb';
  src: url('./assets/fonts/Raleway-SemiBold.ttf')
}
@font-face{
  font-family: 'rale-m';
  src: url('./assets/fonts/Raleway-Medium.ttf')
}
@font-face{
  font-family: 'open-r';
  src: url('./assets/fonts/OpenSans-Regular.ttf')
}
@font-face{
  font-family: 'open-b';
  src: url('./assets/fonts/OpenSans-Bold.ttf')
}
@font-face{
  font-family: 'monts';
  src: url('./assets/fonts/Montserrat-Regular.ttf')
}

body{
  font-family: 'rale-r';
}
.container{
  max-width: 1440px;
  width: 100%;
  margin: auto;
}
.hContainer{
  max-width: 1300px;
  width: 100%;
  margin: auto;
}

button:focus{
  outline: 0;
}
button:hover{
  cursor: pointer;
}
a{
  color: #000;
  text-decoration: none;
}
li{
  list-style: none;
}

.header{
  padding-top: 40px;
  display: flex;
  align-items: center;
  &_links{
  display: flex;
  justify-content: space-between;
  width: 388px;
  margin-left: 615px;
  &_link{
    font-family: 'rale-b';
    line-height: 26px;
    line-height: 26px;
    a{
      position: relative;
      &:hover {
        &::before{
          width: 100%;
        }
      }
      &::before{
      content: '';
      bottom: -4px;
      display: inline-block;
      position: absolute;
      left: 0;
      width: 0%;
      transition: 0.3s;
      height: 1.5px;
      background-color: #FF0019;
        }
      }
    }
  }
  &_lang{
    margin-left: auto;
    display: flex;
    &_btn{
      font-family: 'rale-b';
      font-size: 16px;
      border: 0;
      line-height: 26px;
      background: 0;
      padding: 6px 7px 4px 7px;
      color: #C4C4C4;
      &:first-child{
        margin-right: 20px;
      }
      &:hover{
        border: 1px solid #FF0019;
        border-radius: 50%;
        color: #000;
      }
      &:focus{
        border: 1px solid #FF0019;
        border-radius: 50%;
        color: #000;
      }
    }
  }
}


</style>

<script>
import '@splidejs/splide/dist/css/themes/splide-default.min.css';
export default {
  // new Vue({
  // el: '#app',
  // })
}
</script>