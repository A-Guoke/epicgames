<!-- 一个导航栏 -->
<template>
    <header class="wrapper">
    <nav>

        <input type="radio" name="tab" id="home" checked>
        <input type="radio" name="tab" id="user">
        <input type="radio" name="tab" id="message">
        <input type="radio" name="tab" id="collect">
        <input type="radio" name="tab" id="create">
        <div class="tab"></div>
        <label for="home" class="home"><a href="#"><i class="fa fa-home"></i>首页</a></label>
        <label for="user" class="user"><a href="#"><i class="fa fa-user"></i>用户</a></label>
        <label for="message" class="message"><a href="#"><i class="fa fa-bell"></i>消息</a></label>
        <label for="collect" class="collect"><a href="#"><i class="fa fa-star"></i>收藏</a></label>
        <label for="create" class="create"><a href="#"><i class="fa fa-pencil"></i>创作</a></label>
    </nav>
    </header>
</template>
<style>

:root {
    --navheight: 40px;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-size: 14px;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}


.wrapper {
    height: var(--navheight);
    line-height: var(--navheight);
    border-radius: var(--navheight);
    width: 55vw;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.25);
    overflow: hidden;
}

.wrapper nav {
    display: flex;
    position: relative;
}

.wrapper nav label {
    position: relative;
    flex: 1;
    text-align: center;
    z-index: 2;
    color: #666;
}

.wrapper nav label i { 
    margin: 0 5px;
}

.wrapper nav label a {
    color: #666;
    pointer-events: none;
    text-decoration: none;
    transition: 0.6s;
}

#home:checked ~ label.home a ,
#user:checked ~ label.user a ,
#message:checked ~ label.message a ,
#collect:checked ~ label.collect a ,
#create:checked ~ label.create a {
    color: #fff;
}

.wrapper nav .tab {
    position: absolute;
    height: 100%;
    width: 20%;
    top: 0;
    left: 0;
    background: linear-gradient(45deg, #fc6076 0%, #ff9a44 100%);
    border-radius: var(--navheight);
    transition: .6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}


#user:checked ~ .tab { left: 20% }
#message:checked ~ .tab { left: 40% }
#collect:checked ~ .tab { left: 60% }
#create:checked ~ .tab { left: 80% }


.wrapper nav input {
    display: none;
}
</style>