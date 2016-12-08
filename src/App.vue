<template>
  <div id="app">
    <home></home>
  </div>
</template>

<script>
  import Home from './components/Home'

  export default {
    name: 'app',
    components: {
      Home
    }
  }
</script>

<style lang="scss">
  .icon-heart{
    width: 15px;
    height: 13px;
    display: inline-block;
    background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC0AAAAnCAYAAACbgcH8AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAbxJREFUeNrs2NFNwzAQANDEE2SEdIOwAZ2g8MMPQmomACaATBB1gkRC/PBDOgHdgGxQRvAI3FWHZNLYteNrZEs96VSpSs6v19bJJU0M8fH+lsHLDeQKsoDMRw7bQW4hu7v7hx9DrVypdT1yCJ7bK7WkrlZqwD5BPkJmiX20kJWKJ+wL5NqhDoI3UOfVCg2LYEc/NV21XfAZFmyhFkJrxw8+7P4t1Oq1aFgEv77GY5HhgjlDHWxCCfDuCE0d/mICcwfCl38dT5Xf8D5QsApf4B9U0Bt14OCEfPWh0/Tv3ifxxEI4bkUhxFrQZh9TrARd6WKKQiQRxgV9QZ9A7yIzd4LuX2OKraB7YBkJWB46TRPCJhI0DgZSvTX9DvxC0wP4arh7lAH/TCT5RieXEAeBfwOAaUYMBX4ENk3jIcBHwVp0AHAt2HgZpxOW9ABl1l3CBDZ2Wul4Rh0vZgQbd7HUptJMcCuwNXoGuDXYCX1GuBPYGa3gG6YpvgVs6XpSOnU1BvgksBfaEz4Z7I2eCPcCs8yIBKgsD698wSydVjqO3W4Mh+Az5pZjLTb0CTgbmB2tgbOCz4IewNnBGL8CDAAwErTF4SgCKwAAAABJRU5ErkJggg==);
    background-repeat: no-repeat;
    background-size: contain;
  }

  $pebbleDarkGrey: #303030;

  #app {
    font-family: 'PFDinDisplayProRegularWebfont',sans-serif !important;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  body {
    background-color: $pebbleDarkGrey !important;
  }
</style>
