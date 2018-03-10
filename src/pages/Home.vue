<template>
  <div class="home">
    <div class="header">
      <div class="container">
        <div class="header-nav">
          <div class="row">
            <div class="col-lg-2">
              <router-link to="/">
                <img src="../assets/images/logo.png" alt="logo"/>
              </router-link>
            </div>
            <div class="col-lg-10">hihihi</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script src="./js/home.js"></script>
<style lang="scss" scoped>
.home {
  .header {
    min-height: 1000px;
    width: 100%;
    background-size: 100%;
    background-image: url('../assets/images/home.png');
    background-repeat: no-repeat;
    background-clip: content-box;
  }
}
</style>
