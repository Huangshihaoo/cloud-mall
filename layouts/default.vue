<template>
  <div class="layout">
    <header class="header container">
      <div class="logo">网易云音乐*商城</div>
      <div class="right">
        <div class="search">
          <input type="text" placeholder="蓝牙耳机">
        </div>
        <div class="cart">
          <div class="dot">0</div>
        </div>
        <div class="login">登录</div>
      </div>
    </header>
    <slot></slot>
    <footer class="footer">
      <div class="main container">
        <div class="left">
          <p class="links">
            <a href="/">服务条款</a>｜<a href="/">隐私政策</a>｜<a href="/">儿童隐私政策</a>｜<a href="/">版权投诉指引</a>｜<a href="/">联系我们</a>
          </p>
          <p class="txt">网易公司版权所有©1997-2023杭州乐读科技有限公司运营：浙网文[2021] 1186-054号</p>
          <p class="txt">食品经营许可证 出版物经营许可证 营业执照 网络食品交易第三方平台提供者信息备案: 浙网食A33010041 进口冷链管理承诺书</p>
          <p class="txt">粤B2-20090191-18举报邮箱：工业和信息化部备案管理系统网站</p>
        </div>
        <div class="right"></div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 80px;
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

  .right {
    display: flex;
    justify-content: space-between;

    .search {
      width: 300px;
      height: 36px;
      padding: 1px 30px;
      box-sizing: border-box;
      background-image: url(@/assets/images/modules.png);
      background-repeat: no-repeat;
      background-position: 0px 0px;

      input {
        background: none;
        border: none;
        outline: none;
        padding: 0;
        width: 100%;
        height: 100%;
      }
    }

    .cart {
      position: relative;
      width: 33px;
      height: 33px;
      margin: 0 40px;
      background-image: url(@/assets/images/modules.png);
      background-position: -111px -159px;
      cursor: pointer;

      .dot {
        position: absolute;
        top: -10px;
        right: -10px;
        width: 20px;
        height: 20px;
        border-radius: 10px;
        text-align: center;
        line-height: 20px;
        color: #fff;
        background-image: url(@/assets/images/modules.png);
        background-position: -155px -157px;
      }
    }

    .login {
      cursor: pointer;
    }
  }
}

.footer {
  height: 160px;
  background-color: #f2f2f2;

  .main {
    padding-top: 10px;
    display: flex;
    justify-content: space-between;

    .left {
      .links {
        color: #999;

        a {
          text-decoration: none;
          color: #999;
        }
      }
    }
  }
}
</style>