<template>
<div>
  <div>
<b-container fluid>
<div classs="background">
  <b-navbar toggleable="lg" type="dark">
       <Sidebar/>
    <b-navbar-brand href="#" class="brand">Dashboard</b-navbar-brand>
     <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
         <b-collapse id="nav-collapse" is-nav>
                  <b-form-input size="sm" class="mr-sm-2 search-box" placeholder="Search"></b-form-input><b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto header_icon" >

          <!-- Using 'button-content' slot -->
          <b-button class="btn btn-neutral btn-sm">New</b-button>
            <b-button class="btn btn-neutral btn-sm">Filter</b-button>
              <b-button @click="Logout" class="btn btn-neutral btn-sm">Log-Out</b-button>
                 </b-navbar-nav>
                 
    </b-collapse>
  </b-navbar>
</div>
</b-container>
</div>
</div>
</template>
<script>
export default{
    name: 'header_demo',
     methods: {
    Logout() {
      localStorage.clear();
      this.$router.push({ name: "login" });
    },
  },
}
</script>
<style scoped>
.form-control {
    display: block;
        width: 20%;
    }
.navbar-toggler {
    padding: 0.2rem 0.35rem !important;
    font-size: 1.2rem !important;
    line-height: 1;
    border-radius: 0.25rem;
}
.header_icon{
  color:rgb(42, 82, 114);
  margin-left: auto;
}
 .navbar-brand {
    color:white;
        font-size: 1.1rem !important;
            margin-left: 26px;
}
.nav-items{
  padding: 5px;
}
.brightness{
  padding: 7px;
  margin-right: 5px;
  border-radius: 25%;
 background-color: rgb(27, 27, 73);
  color:gray;
  vertical-align: middle !important;
  font-size: 30px;
  position: relative;
}
.circle{
      position: absolute;
    font-size: 3.8em;
    color: red;
    top: -5px;
    left: 10px;
}
.brightness:hover{
   color:rgb(39, 124, 184);
}
.search-box[data-v-1a9bb128] {
    position: absolute;
    top: 50%;
    left: 29%;
    transform: translate(-50%, -50%);
    background-color: transparent;
    border: 1px solid #bdbcbc;
    height: 40px;
    border-radius: 40px;
    padding: 10px;
    display: flex;
    width: 220px;
    color:white;
    justify-content: space-between;
}
.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    margin-right: 7px;
    position: relative;
    text-transform: none;
    transition: all .15s ease;
    letter-spacing: .025em;
    font-size: .875rem;
}
.btn:hover {
    box-shadow: 0 7px 14px rgb(50 50 93 / 10%), 0 3px 6px rgb(0 0 0 / 8%);
    transform: translateY(-1px);
}

.btn-neutral, .btn-neutral:hover {
    color: #212529;
    background-color: #fff;
    border-color: #fff;
}
.btn-sm {
    padding: 0.25rem 0.5rem;
    line-height: 1.5;
    border-radius: 0.25rem;
}
@media (max-width: 1024px){
  .search-box[data-v-1a9bb128] {
     left: 38%;
  }
  .b-sidebar {
    display: flex;
    flex-direction: column;
    position: fixed;
    top: 0;
    width: 250px;
  }
}
</style>