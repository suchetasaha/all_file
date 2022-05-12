<template>
     <div>
        <b-container fluid>
  <b-navbar toggleable="lg" type="dark" variant="light">
 <b-container>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Home</b-nav-item>
         <b-nav-item href="#">Login</b-nav-item>
          <b-nav-item href="#" @click="logout">Log-out</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
 </b-container>
  </b-navbar>
        </b-container>
</div>
</template>
<script>
export default {
name: 'header-file',
methods:{
    logout(){
         console.log('Sucessfully logout.')
    }
}
}
</script>
<style scoped>
.container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    width: 100%;
 padding-right: 0!important;
    padding-left: 0 !important;}

    .navbar-dark .navbar-nav .nav-link {
    color: black;
    font-weight: bold;}
    
    .navbar-expand-lg .navbar-nav .nav-link {
    padding-right: 1rem !important;
    padding-left: 1rem !important;}
    
</style>