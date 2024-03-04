<script >

</script>

<template>
  <main>
    <div class="m-auto w-4/5">
        <div class="text-3xl font-bold">購買確認及填寫資訊</div>
        <div class="grid grid-cols-4 items-center py-6 border-t-2 border-b-2 border-solid border-black">
            <div><img src="../assets/image/300x300_1.png" style="width: 100px; height: 100px;" alt=""></div>
            <div><h3>Bytecard</h3></div>
            <div class="mr-2">數量:</div>
            <div class="bottom">價格: 954</div>
        </div>
        <div class="mt-6">
            <div class="font-bold">姓名</div>
            <input class="input" type="text">
        </div>
        <div class="mt-2">
            <div class="font-bold">電話</div>
            <input class="input" type="text">
        </div>
        <div class="mt-2">
            <div class="font-bold">地址</div>
            <input class="input" type="text">
        </div>
        <div class="mt-2">
            <div class="font-bold">電子信箱</div>
            <input class="input" type="text">
        </div>
        <div class="mt-4">
            <div class="font-bold">付款方式</div>
            <div class="flex mt-4 gap-4">
                <div><input type="radio" name="bbb">信用卡</div>
                <div><input type="radio" name="bbb">貨到付款</div>
            </div>
        </div>
        <div class="mt-4">
            <div class="font-bold">運送方式</div>
            <div class="flex mt-4 gap-4">
                <div><input type="radio" name="aaa">宅配</div>
                <div><input type="radio" name="aaa">超商取貨</div>
            </div>
        </div>
        <div class="flex items-end flex-col">
            <div class="text-2xl font-bold">商品數量：</div>
            <div class="text-2xl font-bold">商品金額：＄</div>
        </div>
        <div class="flex justify-between">
            <RouterLink to="/check"><div class="bg-indigo-500 px-5 rounded-md text-white">回上頁繼續加購</div></RouterLink>
            <RouterLink to="/ok"><div class="bg-indigo-500 px-5 rounded-md text-white">確認送出</div></RouterLink>
        </div>
    </div>
  </main>
</template>
<style scoped>
.input{
    width: 100%;
    border: 3px solid black;
    margin-top: 10px;
    border-radius: 10px;
}
</style>