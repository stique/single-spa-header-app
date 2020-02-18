<template>
  <div id="vue-app">
      <div id="vue-component" class="container">
          <div class="main">
            <p>
                Header
            </p>
            <p id="links">
                <router-link to="/">List</router-link>
                <router-link to="/detail">Detail</router-link>
            </p>
            <router-view></router-view>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {},
};
</script>

<style lang="scss" scoped>
#vue-component {
  display: block;

  .main{
    #links{
      margin: 30px 0 30px;
      a{
        padding: 10px;
        display: inline-block;
        width: 75px;
        text-align: center;

        &.router-link-exact-active{
          background-color: #007bff;
          color: #fff;
          border-radius: 4px;
        }
      }
    }
  }
}
</style>
