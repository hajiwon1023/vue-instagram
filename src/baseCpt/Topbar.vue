<template>
  <div class="header-topbar">
    <div class="topbar">
      <div class="topbar-container">
        <div class="topbar-left">
          <div class="topbar-left-icon topbar-left-icon-camera"></div>
        </div>
        <div class="topbar-center">
          <div class="topbar-center_index"></div>
        </div>
        <div class="topbar-right">
          <i class="iconfont iconfontIns-icon_send_plane"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
    };
  },
  methods: {
  },
};
</script>

<style scoped>
.header-topbar {
  height: 88px;
  background-color: var(--color-white);
}
.topbar {
  position: fixed;
  z-index: 10;
  top: 0;
  left: 0;
  width: 100%;
  height: 88px;
  background-color: var(--color-bar);
  &::before {
    background: var(--border-gray);
    content: '';
    height: 1px;
    left: 0;
    position: absolute;
    right: 0;
    bottom: -1px;
  }
  &-container {
    display: flex;
    height: 100%;
    padding: 0 var(--padding-lr);
    align-items: center;
  }
  &-left {
    height: auto;
    flex-basis: 60px;
    text-align: center;
    &-icon {
      display: inline-block;
      width: 49px;
      height: 58px;
      background-image: url(../assets/images/icon-sprite.png);
      background-size: 704px 676px;
      &-camera {
        background-position: -554px -165px;
      }
    }
  }
  &-center {
    flex-grow: 1;
    text-align: center;
    &_index {
      display: inline-block;
      vertical-align: middle;
      height: 58px;
      width: 206px;
      background-image: url(../assets/images/icon-sprite.png);
      background-size: 704px 676px;
      background-position: -242px -352px;
    }
  }
  &-right {
    flex-basis: 60px;
    .iconfont {
      font-size: 50px;
    }
  }
}
</style>
