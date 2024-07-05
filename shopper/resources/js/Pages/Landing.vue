<script setup>
import Button from "primevue/button";
import IconField from "primevue/iconfield";
import InputIcon from "primevue/inputicon";
import InputText from "primevue/inputtext";
import Rating from 'primevue/rating';
import { ref } from 'vue';

const value = ref(4);
</script>

<template>
  <div class="w-screen montserrat">
    <div class="h-[888px] relative w-full">
      <div class="w-full px-20 h-[63px] mt-6 flex justify-between items-center">
        <img src="/svg/shopper_logo.svg" alt="" />
        <div class="flex gap-8 items-center">
          <IconField>
            <InputIcon class="pi pi-search" />
            <InputText class="h-[60px] w-[347px]" placeholder="Search" />
          </IconField>
          <Button
            class="w-[247px] h-[60px]"
            icon="pi pi-shopping-cart"
            label="0 items added"
          />
          <Button
            class="w-[247px] h-[60px]"
            icon="pi pi-user"
            label="Login or Sign up"
          />
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
          class="absolute top-[710px] right-[761px] flex flex-col justify-center items-center font-[500]"
        >
          <img src="/svg/playvideo.svg" alt="" />
          <p>Play video</p>
        </div>
        <img
          class="absolute top-[250px] right-[628px]"
          src="/svg/star.svg"
          width="53px"
          alt=""
        />
        <img
          class="absolute bottom-[180px] right-[151px]"
          src="/svg/star.svg"
          width="53px"
          alt=""
        />
      </div>
    </div>
    <div class="h-[680px] flex relative bg-[#845EC2]">
      <div
        class="w-7/12 flex flex-col justify-between items-center "
      >
        <p class="text-[70px] font-[800] mt-20 text-white outline-2 stroke-slate-950">Apple wireless Airpod</p>
        <div class="w-full flex gap-[32px] absolute top-40 justify-center items-end h-[470px]">
          <div
            class="bg-cover w-[189px] h-[331px] bg-center rounded-t-full rounded-b-full"
            style="
              background-image: url(/img/3a1ce3f43d18044f08f9b1d7ba5230bf.png);
            "
          ></div>
          <div
            class="bg-cover place-self-start w-[189px] h-[331px] bg-center rounded-t-full rounded-b-full"
            style="
              background-image: url(/img/38f276464389dfe88e6fd15e032f9a60.png);
            "
          ></div>
          <div
            class="bg-cover w-[189px] h-[331px] bg-center rounded-t-full rounded-b-full"
            style="
              background-image: url(/img/16a33b1a000578efa171337ae6a6e018.png);
            "
          ></div>
        </div>
        <p class="text-[40px] pb-5 text-white">Price : $49.99</p>
      </div>
      <div class="w-4/12 text-white flex flex-col justify-center items-start gap-10 ">
        <p class="text-[50px] font-[700] w-[600px]">Our Featured products</p>
        <p class="font-[500] text-[21px] w-[500px]">Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a product</p>
        <div class="w-full flex justify-around items-center">
          <Button
            class="w-[263px] h-[70px]"
            icon="pi pi-shopping-cart"
            label="Add to card"
          />
          <Button
            class="w-[247px] h-[60px]"
            severity="secondary"
            icon="pi pi-user"
            label="View more"
          />
        </div>
      </div>
    </div>
    <div class=" h-[829px] mt-20 w-full ">
        <p class="text-center text-[44px] font-[600]">Top sellers</p>
        <div class="w-full flex text-[26px] space-x-5 mt-5 font-[600] justify-center items-center">
            <p class="bg-[#10B981]  rounded-full p-8 text-white  ">Top Picks</p>
            <p>Watches</p>
        </div>
        <div class="grid h-[500px] mt-20 grid-cols-3 gap-16 px-40">
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/258d2895eaafe1948111390bead0b9ee.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/932316f9614920ca6f56ae8aa5e219f7.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/aba819e6ef43e086604c73efc97bdfde.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
        </div>
    </div>
    <div class=" h-[829px] mt-40 w-full ">
        <p class="text-center text-[44px] font-[600]">Top sellers</p>
        <div class="w-full flex text-[26px] space-x-5 mt-5 font-[600] justify-center items-center">
            <p class="bg-[#10B981]  rounded-full p-8 text-white  ">Top Picks</p>
            <p>Watches</p>
        </div>
        <div class="grid h-[500px] mt-20 grid-cols-3 gap-16 px-40">
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/258d2895eaafe1948111390bead0b9ee.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/932316f9614920ca6f56ae8aa5e219f7.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
          <div class="h-[600px]">
            <div class="bg-[#ECFEF4] p-10 h-full flex flex-col justify-center items-center gap-4   rounded-xl">
              <img src="/img/aba819e6ef43e086604c73efc97bdfde.png" class="h-1/2" alt="">
              <div class="h-1/2 bg-gray-100 rounded-3xl p-12 flex flex-col justify-around items-start  w-full ">
                <p class="text-[30px] font-[500]">Boat Rockerz 333</p>
                <Rating v-model="value"  readonly />
                <p class="text-[21px] font-[500]">$55</p>
              </div>
            </div>
            <Button class="w-full mt-8 h-16" label="Add to card"  />
          </div>
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

