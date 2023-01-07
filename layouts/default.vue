<template>
    <div class="layout">
        <header class="header container">
            <div class="logo">网易云音乐*商城</div>
        </header>
        <slot></slot>
        <footer class="footer container"></footer>
    </div>
</template>

<style lang="scss" scoped>
.header {
    height: 80px;
    line-height: 80px;
    background-color: #fff;

    .logo {
        display: inline-block;
        width: 300px;
        height: 40px;
        margin-top: 20px;
        background-image: url(@/assets/images/modules.png);
        background-repeat: no-repeat;
        background-position: 0px -63px;
        font-size: 0px;
    }
}
</style>