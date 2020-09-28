<template>
  <div id="app">
    <NavigationMobile v-if="mobileView && showNav" />
    <div class="content" :class="{'open':showNav}">
      <div class="top-bar">
        <div id="navigation-icon" v-if="mobileView"
          @click="showNav = !showNav">
          <i class="fas fa-bars"></i>
        </div>
        <Navigation v-if="!mobileView" />
      </div>
    </div>
    <Container class="journey-section">
      <h2>Zaplanuj wycieczkę</h2>
      <div class="journey-section--custom-background">
         <Tabs>
            <Tab name="Wszystkie">
            <div class="pointer-container">
            <div class="pointer-container--pointer"></div>
            </div>
      </Tab>
      <Tab name="Z rodziną" selected="true">
            <div class="pointer-container">
            <div class="pointer-container--pointer"></div>
            </div>
      </Tab>
      <Tab name="Miasta">
            <div class="pointer-container">
            <div class="pointer-container--pointer"></div>
            </div>
      </Tab>
      <Tab name="Unesco">
            <div class="pointer-container">
            <div class="pointer-container--pointer"></div>
            </div>
      </Tab>
    </Tabs>
    </div>
    </Container>
    <Container>
    <h2>Atrakcje regionu</h2>
<hooper group="group1" :itemsToShow="4" :settings="hooperSettings">
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
</hooper>

<hooper group="group1" :itemsToShow="4" :settings="hooperSettings">
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>
  <slide>
    <div class="card-container">
    <div class="card-container--image-holder">
    <img src="@/assets/adventure-park.jpg"/>
    </div>
    <div class="card-container--text-holder">
    <div class="card-container--text-holder--header">Just lorem ipsum</div>

    <a href="#" class="main-btn">Dowiedz się więcej</a>
    </div>

    </div>
  </slide>

  <hooper-navigation slot="hooper-addons"></hooper-navigation>
</hooper>
</Container>
  </div>
</template>

<script>
import Container from './components/Container.vue'
import Navigation from './components/Navigation.vue'
import NavigationMobile from './components/NavigationMobile.vue'
import Tabs from './components/Tabs.vue'
import Tab from './components/Tab.vue'
import { Hooper, Slide, Navigation as HooperNavigation } from 'hooper'
import 'hooper/dist/hooper.css'
export default {
  data: () => {
    return {
      mobileView: true,
      showNav: false,
      hooperSettings: {
        itemsToShow: 2,
        breakpoints: {
          990: {
            itemsToShow: 4
          }
        }
      }
    }
  },
  methods: {
    handleView () {
      this.mobileView = window.innerWidth <= 990
    }
  },
  components: {
    Container,
    Navigation,
    NavigationMobile,
    Tabs,
    Tab,
    Hooper,
    Slide,
    HooperNavigation
  },
  created () {
    this.handleView()
    window.addEventListener('resize', this.handleView)
  }
}
</script>

<style lang="scss">
@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

img {
max-width:100%;
}

.main-btn {
    border: 2px solid #dcdcdc;
    background: #fff;
    font-size: 12px;
    font-weight: 500;
    display: inline-block;
    text-transform: uppercase;
    cursor: pointer;
    width: fit-content;
    padding: 10px 15px;
    text-decoration: none;
}

.journey-section {
margin-top:50px;
&--custom-background {
background-color:#d3d3d3;
height:300px;
position:relative;
margin-top:90px;
}
}

.pointer-container {

&--pointer {
height:5px;
width:5px;
background-color:red;
}
}

.hooper {
height:400px;
margin-bottom:30px;
.card-container {
height:inherit;
margin-left:15px;
margin-right:15px;
border-left: 1px solid #dcdcdc;
border-right: 1px solid #dcdcdc;
border-top: 1px solid #dcdcdc;
border-bottom: 3px solid #009e5f;
&--image-holder {
height:50%;
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
}
}
&--text-holder {
    height: 50%;
    width: 100%;
    display: flex;
    padding:20px;
    flex-direction: column;
    justify-content: space-between;
}
}
}

#app {
  position: relative;
  padding: 10px;
  color: #333;
  overflow: hidden;
}
.top-bar {
  display: flex;
  width: 100%;
}
#navigation-icon {
  padding: 10px 10px 20px;
  margin-right: 10px;
  cursor: pointer;
  i {
    font-size: 2rem;
  }
}
.content {
  position: absolute;
  top: 10px;
  padding: 20px;
  transition: 1s transform cubic-bezier(0,.12,.14,1);
  left:0;
  right:0;
}
.open {
  transform: translateX(300px);
}
</style>
