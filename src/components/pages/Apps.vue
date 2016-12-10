<template>
  <div class="category-menu">
    <div class="row">
      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-daily.png" />
        <p class="color-daily">Daily</p>
      </div>

      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-tools.png" />
        <p class="color-tools">Tools & Utilities</p>
      </div>
    </div>

    <div class="row">
      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-notifications.png" />
        <p class="color-notifications">Notifications</p>
      </div>

      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-remotes.png" />
        <p class="color-remotes">Remotes</p>
      </div>
    </div>

    <div class="row">
      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-health.png" />
        <p class="color-health">Health & Fitness</p>
      </div>

      <div class="col-xs-6 app-category">
        <img class="category-image float-xs-left" src="../../assets/category-games.png" />
        <p class="color-games">Games</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'apps'
  }
</script>

<style lang="scss" scoped>
  $color-daily: #3db9e6;
  $color-tools: #fdbf37;
  $color-notifications: #FF9000;
  $color-remotes: #fc4b4b;
  $color-health: #98D500;
  $color-games: #b57ad3;

  $pebbleMedGrey: #484848;
  $pebbleOrange: #ff4700;

  .color-daily {
    color: $color-daily;
  }

  .color-tools {
    color: $color-tools;
  }

  .color-notifications {
    color: $color-notifications;
  }

  .color-remotes {
    color: $color-remotes;
  }

  .color-health {
    color: $color-health;
  }

  .color-games {
    color: $color-games;
  }

  .category-menu {
    width: 100%;
    border-top: 2px solid $pebbleOrange;
    border-bottom: 2px solid $pebbleOrange;
    background-color: $pebbleMedGrey;

    .app-category {
        img {
          width: 34px;
          height: auto;
        }

        p {
          padding-top: 10px;
          margin-left: 40px;
          text-transform: uppercase;
        }
    }
  }

</style>
