<template>
  <div>
    <b-button v-b-toggle.sidebar-1> <b-icon icon="list" class="side-icon" aria-hidden="true"></b-icon></b-button>
    <b-sidebar id="sidebar-1" title="Sidebar" shadow>
      <div class="px-3 py-2">
        <nav>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="house-door-fill" class="menu"></b-icon><NuxtLink to="/">Home page</NuxtLink>
          </div>
        </b-nav-items>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="bar-chart-fill" class="menu"></b-icon><NuxtLink to="/dashboard">Dashboard</NuxtLink>
          </div>
        </b-nav-items>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="gift" class="menu"></b-icon> <NuxtLink to="/form">Form</NuxtLink>
          </div>
        </b-nav-items>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="layout-text-sidebar" class="menu"></b-icon><NuxtLink to="/table">Table</NuxtLink>
          </div>
        </b-nav-items>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="gear" class="menu"></b-icon><NuxtLink to="/Modal">Modal</NuxtLink>
          </div>
        </b-nav-items>
        <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="person" class="menu"></b-icon><NuxtLink to="/wizard">Wizard</NuxtLink>
          </div>
        </b-nav-items>
          <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="gift" class="menu"></b-icon>  <NuxtLink to="/Webpage">Web-Page</NuxtLink>
          </div>
        </b-nav-items>
          <b-nav-items href="#">
          <div class="icon">
            <b-icon icon="gift" class="menu"></b-icon> <NuxtLink to="/login">Login</NuxtLink>
          </div>
        </b-nav-items>
      </nav>
      </div>
    </b-sidebar>
  </div>
</template>
<script>
export default {
    name:'side-bar'
}
</script>
<style scoped>
.side-icon{
     color: black;
  font-size: 25px;
}
.btn-secondary {
    color: #fff;
    background-color: #6c757d;
    border-color: none !important;
}
.btn-secondary {
    color: #fff;
     background-color: transparent; 
    border-color: #6c757d;
}
.icon{
  color: rgb(27, 27, 73) !important;
  padding-bottom:10px;

}
label {
    display: inline-block;
    margin-bottom: 0.5rem;
    margin-left: 20px;
     color: rgb(27, 27, 73);
}
.menu{
  font-size: 1.2rem;
   margin-right: 13px;
}
.b-sidebar {
    display: flex;
    flex-direction: column;
    position: fixed;
    top: 0;
    width: 220px !important;
    max-width: 100%;
    height: 100vh;
    max-height: 100%;
    margin: 0;
    outline: 0;
    transform: translateX(0);
}
</style>