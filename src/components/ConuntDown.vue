<template>
    <div class="dateBox">
        <div class="date-item">
            <div class="time">{{ state.day }}</div>
            <div class="label">天</div>
        </div>
        <div class="date-item">
            <div class="time">{{ state.hours }}</div>
            <div class="label">时</div>
        </div>
        <div class="date-item">
            <div class="time">{{ state.minutes }}</div>
            <div class="label">分</div>
        </div>
        <div class="date-item">
            <div class="time">{{ state.seconds }}</div>
            <div class="label">秒</div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { reactive, onMounted } from 'vue';

const props = defineProps({
  targetTime: {
    type: Number,
    require: true,
    default: 0
  }
});

const state = reactive({
    day: 0,
    hours: 0,
    minutes: 0,
    seconds: 0
});

// 定时器实例
let intervalId: any; 

const dateCountDown = () => {
    let nowTime = new Date().getTime(); //现在时间
    let diff:number = props.targetTime - nowTime; //目标时间 - 现在时间 计算时间差
    if(diff <= 0){
        clearInterval(intervalId); //时间到期，关闭定时器
    }
    state.day = Math.floor(diff / (1000 * 60 * 60 * 24));
    state.hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
    state.minutes = Math.floor((diff / (1000 * 60)) % 60);
    state.seconds = Math.floor((diff / 1000) % 60);
}

onMounted(() => {
    intervalId = setInterval(dateCountDown, 1000); //初始化倒计时
});
</script>

<style scoped>
.dateBox{
    display: flex;
    justify-content: center;
}
.date-item{
    display: flex;
    align-items: center;
    font-size: 24px;
    font-weight: bold;
}
.time{
    color: red;
}
</style>

