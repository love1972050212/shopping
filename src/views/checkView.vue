<script >

</script>

<template>
  <main>
    <div class="w-4/5 m-auto">
        <div><h1 class="text-3xl font-bold">購物車確認</h1></div>
        <div class="grid grid-cols-5 items-center py-6 border-t-2 border-b-2 border-solid border-black">
            <div><input type="checkbox" name="" id=""></div>
            <div><img src="../assets/image/300x300_1.png" style="width: 100px; height: 100px;" alt=""></div>
            <div><h3>Bytecard</h3></div>
            <div class="mr-2">數量:</div>
            <div class="bottom">價格: 954</div>
        </div>
        <div class="flex justify-end"><h1 class="text-2xl font-bold">商品數量：</h1></div>
        <div class="flex justify-end"><h1 class="text-2xl font-bold">商品總金額：＄</h1></div>
        <div class="flex justify-between">
            <div><RouterLink to="/"><h1 class="text-xl bg-fuchsia-400 text-fuchsia-50 rounded-md">回上頁繼續購買</h1></RouterLink></div>
            <div><RouterLink to="/buy"><h1 class="text-xl bg-fuchsia-400 text-fuchsia-50 rounded-md">確認購買</h1></RouterLink></div>
        </div>
    </div>
    </main>
</template>
<style>
</style>