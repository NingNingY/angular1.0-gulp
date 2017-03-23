<template>
  <div id="app">
    <div class="page-app">
      <div class="bg-success">
        <div class="nav nav-pills ">
            <ul class="list-unstyled list-inline app-nav pull-right">
              <li class="text-uppercase" role="presentation">
                <router-link to="/home"><strong>home</strong></router-link>
              </li>
              <li class="text-uppercase" role="presentation">
                <router-link to="/about"><strong>about</strong></router-link>
              </li>
               <li class="text-uppercase" role="presentation">
                <router-link to="/filter"><strong>filter</strong></router-link>
              </li>
            </ul>
        </div>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>
<script>
export default {
  name: 'app'
}
</script>

<style scoped>
#app {

  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-top: 10px;
}

.page-app {
  width: 100%;
}
.page-app .app-nav {
  text-align: center;
  height: 35px;
  line-height: 35px;
  font-size: 18px;
  margin: 10px 200px 0 0;
}

.page-app .app-nav li{width: 100px}

</style>
