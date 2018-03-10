<template>
  <div class="home">
    <div class="header">
      <div class="header__mask"></div>
      <div class="container">
        <div class="header__nav">
          <div class="row">
            <div class="col-lg-2">
              <router-link to="/">
                <img src="~assets/images/logo.png" alt="logo"/>
              </router-link>
            </div>
            <div class="col-lg-10 header__nav-wrapper">
              <ul>
                <li><router-link to="">About</router-link></li>
                <li><router-link to="">Find Your Course</router-link></li>
                <li class="register"><router-link to="">Register</router-link></li>
              </ul>
            </div>
          </div>
        </div>
        <div class="header__text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum lacus vitae
        </div>
      </div>
    </div>
  </div>
</template>
<script src="./js/home.js"></script>
<style lang="scss" scoped>
.home {
  .header {
    min-height: 550px;
    width: 100%;
    background-size: 100%;
    background-image: url('../assets/images/home.png');
    background-repeat: no-repeat;
    background-clip: content-box;
    position: relative;
    .container {
      min-height: 550px;
      position: relative;
    }
    &__mask {
      position: absolute;
      width: 100%;
      height: 100%;
      background-color: rgba(0,0,0,0.5);
    }
    &__nav {
      &-wrapper {
        text-align: right;
        color: #fff;
        ul {
          list-style: none;
          display: inline-block;
          margin: 0;
          padding: 0;
          li {
            display: inline-block;
            padding: 50px 0px 10px;
            color: #fff;
            margin: 0px 40px;
            &.register {
              background-color: #ffa801;
              padding: 50px 20px 10px;
              border-bottom-left-radius: 3px;
              border-bottom-right-radius: 3px;
            }
            a {
              color: #fff;
              transition: color .2s ease;
              position: relative;
              &:hover {
                &::after,
                &::before {
                  width: 100%;
                  left: 0;
                }
              }
              &::after,
              &::before {
                content: '';
                position: absolute;
                top: calc(100% + 5px);
                width: 0;
                right: 0;
                height: 3px;
              }
              &::before {
                transition: width .4s cubic-bezier(0.51, 0.18, 0, 0.88) .1s;
                background: #ffa801;
              }
              &::after {
                transition: width .2s cubic-bezier(0.29, 0.18, 0.26, 0.83);
                background: #F44336;
              }
            }
          }
        }
      }
    }
    &__text {
      font-size: 40px;
      color: #fff;
      font-weight: bold;
      text-align: center;
      position: absolute;
      width: 60%;
      left: 50%;
      top: 50%;
      transform: translate(-50%,-50%);
    }
  }
}
</style>
