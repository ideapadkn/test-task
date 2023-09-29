<template>
  <div>
    <div class="menu">
      <div class="menu__content">
        <div class="menu__content-img">
          <img src="https://img.freepik.com/premium-photo/lake-landscape_967069-28.jpg" alt="">
        </div>
        <div class="menu__content-title">
          Menu Title
        </div>
        <p class="menu__content-text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur, ratione perspiciatis illum magni suscipit,
          vitae qui, ut
        </p>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.menu {
  background-color: rgba(38, 38, 38, 1);
  padding: 18px;
  border-radius: 12px;
  width: 236px;
  display: flex;
  align-items: center;
  flex-direction: column;
  height: 500px;

  &__content {
    text-align: center;

    &-img {
      width: 208px;
      height: 240px;
      margin-bottom: 20px;
    }

    &-title {
      color: #fff;
      font-size: 24px;

    }

    &-text {
      color: #fff;
      font-size: 16px;
      line-height: 150%;
    }
  }
}
</style>