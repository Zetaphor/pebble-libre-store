<template>
  <div id="watchfaces" class="container">
    <div class="row">
      <div class="col-sm-10 offset-sm-1 main-content">
        <div class="row top-nav">
          <p class="main-title">pebble libre</p>
          <div v-on:click="switchPage('watchfaces')" class="col-sm-4 nav-link">
            <p class="text-xs-center" v-bind:class="{ active: showWatchfaces }">
              <svg class="svg-icon" viewBox="0 0 100 100">
                <path d="M50,10.1c22.1,0,39.9,17.9,39.9,39.9c0,22.1-17.9,39.9-39.9,39.9S10.1,72.1,10.1,50
                  C10.1,27.9,27.9,10.1,50,10.1 M50,0C22.4,0,0,22.4,0,50s22.4,50,50,50s50-22.4,50-50S77.6,0,50,0L50,0z">
                </path>
                <polygon points="45,54.8 45,24.9 52.2,24.9 52.2,50.8 74.9,64.7 71.1,70.9 	"></polygon>
              </svg>
              <span>Watchfaces</span>
            </p>
          </div>

          <div v-on:click="switchPage('apps')" class="col-sm-4 nav-link">
            <p class="text-xs-center" v-bind:class="{ active: showApps }">
              <svg class="svg-icon" viewBox="0 0 100 100">
                <path d="M90.6,9.4V73H27V9.4H90.6 M90.6,0H27c-5.2,0-9.4,4.2-9.4,9.4V73c0,5.2,4.2,9.4,9.4,9.4h63.7
                  c5.2,0,9.4-4.2,9.4-9.4V9.4C100,4.2,95.8,0,90.6,0L90.6,0z">
                </path>
                <path d="M82,90.6H9.4V18H0v72.6c0,5.2,4.2,9.4,9.4,9.4H82V90.6z"></path>
              </svg>
              <span>Apps/Timeline</span>
            </p>
          </div>

          <div v-on:click="switchPage('search')" class="col-sm-4 nav-link">
            <p class="text-xs-center" v-bind:class="{ active: showSearch }">
              <svg class="svg-icon" viewBox="0 0 100 100">
                <path d="M99.2,93.8L60.1,54.7c4.8-5.8,7.7-13.2,7.7-21.3C67.8,14.9,52.8,0,34.4,0C15.9,0,1,14.9,1,33.4
                  c0,18.4,14.9,33.4,33.4,33.4c7.2,0,13.8-2.3,19.3-6.2L93.1,100L99.2,93.8z M9.7,33.4c0-13.6,11.1-24.7,24.7-24.7
                  C48,8.7,59,19.8,59,33.4C59,47,48,58,34.4,58C20.8,58,9.7,47,9.7,33.4z">
                </path>
              </svg>
              <span>Search</span>
            </p>
          </div>
        </div>

        <watchfaces v-show="showWatchfaces" class="sub-page sub-page-top-margin"></watchfaces>
        <apps v-show="showApps" class="sub-page"></apps>
        <search v-show="showSearch" class="sub-page"></search>
      </div>
  </div>
</template>

<script>
  import Watchfaces from './pages/Watchfaces'
  import Apps from './pages/Apps'
  import Search from './pages/Search'

  export default {
    name: 'home',
    components: {
      Watchfaces,
      Apps,
      Search
    },
    data () {
      return {
        showWatchfaces: true,
        showApps: false,
        showSearch: false
      }
    },

    methods: {
      switchPage (pageName) {
        switch (pageName) {
          case 'watchfaces':
            this.showWatchfaces = true
            this.showApps = false
            this.showSearch = false
            break
          case 'apps':
            this.showWatchfaces = false
            this.showApps = true
            this.showSearch = false
            break
          case 'search':
            this.showWatchfaces = false
            this.showApps = false
            this.showSearch = true
            break
        }
      }
    }
  }
</script>

<style lang="scss" scoped>
  $pebbleMedGrey: #484848;
  $pebbleOrange: #ff4700;

  #watchfaces {
    margin-top: 2rem;
  }

  .svg-icon {
    font-size: 1em;
    height: 17px;
    color: #FFF;
    vertical-align: middle;
    fill: #FFF;
  }

  .main-content {
    background-color: #F4F3F4;
    border-radius: 10px;

    .sub-page-top-margin {
      margin-top: 1rem;
    }

    .main-title {
      color: #fff;
      padding: 1rem 0 0 1rem;
      font-size: 2rem;
      font-family: 'CenturyGothic',sans-serif !important;
    }

    .top-nav {
      color: #FFF;
      background-color: $pebbleMedGrey;
      border-radius: 5px 5px 0px 0px;

      .nav-link {
        cursor: pointer;
      }

      p {
        margin-bottom: 10px;
        &.active {
          border-bottom: 3px solid $pebbleOrange;
        }
      }
    }
  }
</style>
