<script setup>

</script>

<template>
  <div class="container">
    <div class="menu">
      <div class="menu__content">
        <div class="menu__content-img">
          <svg xmlns="http://www.w3.org/2000/svg" width="208" height="240" viewBox="0 0 208 240" fill="none">
            <g filter="url(#filter0_b_0_68)">
              <rect width="208" height="240" rx="8" fill="white" fill-opacity="0.1" />
            </g>
            <defs>
              <filter id="filter0_b_0_68" x="-12" y="-12" width="232" height="264" filterUnits="userSpaceOnUse"
                color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix" />
                <feGaussianBlur in="BackgroundImageFix" stdDeviation="6" />
                <feComposite in2="SourceAlpha" operator="in" result="effect1_backgroundBlur_0_68" />
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_backgroundBlur_0_68" result="shape" />
              </filter>
            </defs>
          </svg>
        </div>
        <div class="menu__content-title">
          Menu Title
        </div>
        <p class="menu__content-text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur, ratione perspiciatis illum magni suscipit,
          vitae qui, ut facere non doloribus in eveniet ipsum at sed quia. Impedit aliquam quos iste.
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
  margin-bottom: 24px;

  &__content {
    text-align: center;

    &-img {
      width: 208px;
      height: 240px;
      margin-bottom: 20px;
    }

    &-title {
      color: #fff;
      font-size: 32px;

    }

    &-text {
      color: #fff;
      font-size: 18px;
      line-height: 150%;
      width: 190px;
    }
  }
}
</style>