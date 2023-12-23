<!--language: JavaScript-->
<template>
    <!-- 背景 -->
    <div class="back">
        <img src="@/assets/img/640x854.jpg" />

        <!-- 展示栏 -->
        <div class="store">
            <!-- 筛选栏 -->
            <div class="filter">
                <p>类型</p>
                <p>筛选</p>
            </div>
            <!-- 商品栏 -->
            <div class="store-a">
                <!-- 商品 -->
                <div class="store-item" v-for="(item, index) in productList" :key="index">
                    <img src="@/assets/vue.svg" />

                    <div class="store-item-right">
                        <div class="store-item-name">
                            <!-- 商品名 -->
                            <!-- <p>商品名</p> -->
                            <!-- 选择类型 -->
                            <!-- <p>选择类型</p> -->
                            <p>{{ item.name }}</p>
                            <p>{{ item.type }}</p>

                        </div>
                        <!-- 价格 -->
                        <div class="store-item-price">
                            <!-- 价格 -->
                            <!-- <p>价格</p> -->
                            <!-- 数量 -->
                            <!-- <p>数量</p> -->
                            <p>{{ item.price }}</p>
                            <p>{{ item.quantity }}</p>

                        </div>
                    </div>
                </div>

            </div>


        </div>
    </div>
</template>

<script setup lang="ts">

const productList = [
    { name: "商品名1", type: "选择类型1", price: "价格1", quantity: "数量1" },
    { name: "商品名2", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名3", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名4", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名5", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名6", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名7", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名8", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名9", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名10", type: "选择类型2", price: "价格2", quantity: "数量2" },
    { name: "商品名11", type: "选择类型2", price: "价格2", quantity: "数量2" },
]

</script>

<style scoped>
/* 设置页面样式 */
* {
    margin: 0;
    padding: 0;
}

.back {
    width: 100%;
    height: 100%;
    background-color: #000;
    position: fixed;
    top: 0;
    left: 0;
}

.back img {
    width: 100%;
    height: 100%;
}

.store {
    width: 100%;
    height: 70%;
    border-radius: 30px 30px 0 0;
    background-color: #fff;
    position: fixed;
    top: 30%;
    left: 0;
}

.filter {
    height: 5%;
    padding: 10px;
    border: 1px solid #000;
    border-radius: 30px 30px 0 0;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

.store-a {
    height: 95%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    overflow: auto;
}

.store-item {
    width: 49%;
    height: 200px;
    border: 1px solid #000;
    margin-top: 2px;
    display: flex;
}

.store-item img {
    width: 30%;
    height: 100%;
}

.store-item-right {
    width: 70%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}

.store-item-name {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    height: 70%;
}

.store-item-name p {
    font-size: 20px;
    color: #000;
}

.store-item-price {
    display: flex;
    justify-content: space-around;
    height: 30%;
}
</style>