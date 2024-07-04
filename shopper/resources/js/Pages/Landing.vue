<script setup>
import Button from "primevue/button";
import IconField from "primevue/iconfield";
import InputIcon from "primevue/inputicon";
import InputText from "primevue/inputtext";
</script>

<template>
  <div class="w-screen montserrat">
    <div class="h-[888px] w-full">
      <div class="w-full px-20 h-[63px] mt-6 flex justify-between items-center">
        <img src="/svg/shopper_logo.svg"  alt="" />
        <div class="flex gap-8 items-center">
          <IconField>
            <InputIcon class="pi pi-search" />
            <InputText class="h-[60px] w-[347px]" placeholder="Search" />
          </IconField>
          <Button class="w-[247px] h-[60px]" label="Register" />
          <Button  class="w-[247px] h-[60px]" label="Sign in" />
        </div>
      </div>
      <div
        class="w-full font-[600] mt-10 px-20 bg-green-400 h-[81px] flex justify-center items-center gap-[75px] text-xl"
      >
        <p>Features</p>
        <p>Products</p>
        <p>Blog</p>
        <p>About</p>
      </div>
      <div class="flex h-[680px] w-full">
        <div
          class="w-1/2 pl-[85px] py-[120px] h-full flex flex-col justify-between items-start"
        >
          <p class="text-[70px] font-[600] w-[599px] h-[156px]">
            Discover our latest Products
          </p>
          <p class="font-[500] w-[] text-[21px]">
            Lorem ipsum is a placeholder text commonly used to demonstrate the
            visual form of a product
          </p>
          <Button
            label="Buy Now"
            class="h-[70px] w-[263px]"
            raised
            size="large"
          />
        </div>
        <div class="w-1/2 flex justify-center items-center h-full">
          <div
            class="w-[272px] scale-110 mt-20 h-[477px] flex flex-col justify-center items-center gap-[26px]"
            style="background-image: url('/svg/productbg.svg')"
          >
            <img src="/img/7eedb5772a46d96b154fd49c6815d972.png" alt="" />
            <p class="font-[500] text-[18px]">red beats Ml9c2zm/a</p>
            <p class="font-[500] text-[31px]">$50</p>
          </div>
        </div>
        <div
          class="fixed top-[767px] right-[761px] flex flex-col justify-center items-center font-[500]"
        >
          <img src="/svg/playvideo.svg" alt="" />
          <p>Play video</p>
        </div>
        <img class="fixed top-[323px] right-[628px]"  src="/svg/star.svg" width="53px" alt="">
        <img class="fixed bottom-[66px] right-[151px]"  src="/svg/star.svg" width="53px" alt="">
      </div>
    </div>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap");

.montserrat {
  font-family: "Montserrat", sans-serif;
}
</style>
