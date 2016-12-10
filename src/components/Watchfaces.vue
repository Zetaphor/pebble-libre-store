<template>
  <div class="col-xs-9 offset-xs-2 watchfaces">
    <div class="row">
      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>

      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>

      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>

      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>

      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>

      <div class="col-xs-4">
        <div class="card">
          <div class="card-block">
            <p class="card-title text-xs-center">Example Watchface</p>
            <img class="img-fluid mx-auto d-block preview-image" src="https://assets.getpebble.com/api/file/Wn2zo34FTwuUw2lAEHVl/convert?cache=true&fit=crop&w=144&h=168" />
            <p class="card-text text-xs-center">
              <span class="icon-heart"></span>
              <span class="total-hearts">193</span>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'watchfaces'
  }
</script>

<style lang="scss" scoped>
  $pebbleGreyLight: #aaa5a3;
  $pebbleWhite: #F4F3F4;

  .watchfaces {
    background-color: $pebbleWhite;
    border-radius: 0 0 10px 10px;
  }

  .preview-image {
    margin-bottom: 0.75rem;
  }

  .total-hearts {
    color: $pebbleGreyLight;
  }
</style>
