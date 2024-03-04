<script>
export default {
  data() {
    return {
      verticalLayout: false
    };
  }
}
</script>

<template>
  <main>
    <div class="w-4/5 m-auto">
      <div>
        <h1 class="text">商品列表</h1>
      </div>
      <div class="flex justify-end mr-3 mb-3">
        <div class="horizontal-icon" @click="verticalLayout = false">
          <img v-if="!verticalLayout" src="../assets/image/iconl_0.png" alt="">
          <img v-else src="../assets/image/1-1.png" alt="">
        </div>

        <div @click="verticalLayout = true">
          <img v-if="!verticalLayout" src="../assets/image/iconr_01.png" alt="">
          <img v-else src="../assets/image/2-2.png" alt="">
        </div>

      </div>
      <div></div>
      <div class="all-container gap-4" v-if="!verticalLayout">
        <div class="container">
          <div><img src="../assets/image/300x300_1.png" alt=""></div>
          <div>
            <h3>Bytecard</h3>
          </div>
          <div>Immunization not carried out because of caregiver refusal</div>
          <div class="bottom">價格: 954</div>
          <div class="flex">
            <div class="mr-2">數量:</div>
            <div class="reduce flex justify-center">-</div>
            <div class="input"><input class="text-right" style="width: 90px;" type="number"></div>
            <div class="add flex justify-center">+</div>
          </div>
          <div class="my-3 flex justify-center bg-blue-400 rounded-md">
            <div><img src="../assets/image/cart-shopping-solid.svg" style="width: 20px; height: 20px;" alt=""></div>
            <div>加入購物車</div>
          </div>
        </div>
        <div class="container">
          <div><img src="../assets/image/shopcard.jpg" alt=""></div>
          <div>
            <h3>Bytecard</h3>
          </div>
          <div>Immunization not carried out because of caregiver refusal</div>
          <div class="bottom">價格: 954</div>
          <div class="flex">
            <div class="mr-2">數量:</div>
            <div class="reduce flex justify-center">-</div>
            <div class="input"><input class="text-right" style="width: 90px;" type="number"></div>
            <div class="add flex justify-center">+</div>
          </div>
          <div class="my-3 flex justify-center bg-blue-400 rounded-md"><img
              src="../assets/image/cart-shopping-solid.svg" style="width: 20px; height: 20px;" alt="">
            <div>加入購物車</div>
          </div>
        </div>
      </div>
      <div class="all-container aa" v-else>
        <div class="container2 w-full">
          <div>商品圖片</div>
          <div>商品名稱</div>
          <div>商品描述</div>
          <div>價錢</div>
        </div>
        <div class="container2 w-full">
          <div class="my-9"><img src="../assets/image/300x300_1.png" style="width: 100px; height: 100px;" alt=""></div>
          <div>
            <h3>Bytecard</h3>
          </div>
          <div>Immunization not carried out because of caregiver refusal</div>
          <div class="bottom">價格: 954</div>
          <div>
            <div class="flex">
              <div class="mr-2 flex white-space-nowrap">數量:</div>
              <div class="reduce flex justify-center">-</div>
              <div class="input"><input class="text-right" style="width: 90px;" type="number"></div>
              <div class="add flex justify-center">+</div>
            </div>
            <div class="flex mt-2"><img src="../assets/image/cart-shopping-solid.svg" style="width: 20px; height: 20px;"
                alt="">
              <div><button>加入購物車</button></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
h3 {
  font-size: 20px;
  font-weight: 600;
}

.text {
  font-size: 32px;
  font-weight: 800;
}

.container {
  width: 300px;
}

.input {
  width: 90px;
  border: 1px solid black;
}

.reduce {
  border: 1px solid black;
  width: 20px;
  border-radius: 10px 0 0 10px;
}

.add {
  border: 1px solid black;
  width: 20px;
  border-radius: 0 10px 10px 0;
}

.bottom {
  margin-bottom: 30px;
}

.all-container {
  display: flex;
  flex-wrap: wrap;
}

.container2 {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  align-items: center;
  gap: 20px;
}

.horizontal-icon img {
  width: 50px;
  /* 调整图标宽度 */
}

.vertical-icon img {
  height: 50px;
  /* 调整图标高度 */
}

.white-space-nowrap {
  white-space: nowrap;
}
</style>
