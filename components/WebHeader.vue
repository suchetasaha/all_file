<template>
    <div>
        <b-container fluid>
  <b-navbar toggleable="lg" type="dark" variant="light">
         <Sidebar/>
 <b-container>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Home</b-nav-item>
         <b-nav-item href="#">Guide</b-nav-item>
          <b-nav-item href="#">Service</b-nav-item>
           <b-nav-item href="#">Contact</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-button size="sm" class="my-2 my-sm-0 contact" type="submit">Contact Us</b-button>
        </b-nav-form>
        </b-navbar-nav>
    </b-collapse>
 </b-container>
  </b-navbar>
        </b-container>
</div>
</template>
<script>
export default {
name :'header-page'
}
</script>
<style scoped>
.container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    width: 100%;
 padding-right: 0px !important;
    padding-left: 0 !important;
    }
    .navbar-dark .navbar-nav .nav-link {
    color: black;
    font-weight: bold;
    }
    .navbar-expand-lg .navbar-nav .nav-link {
    padding-right: 1rem !important;
    padding-left: 1rem !important;
    }
    .contact{
        background-color: transparent;
        border:2px solid black;
        color:rgb(7, 7, 7);
        padding:5px 27px;
        font-weight: bold;
    }
</style>