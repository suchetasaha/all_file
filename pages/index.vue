<template>
<div>
  <div class="navbar">
   <Sidebar/> 
   <ul class="list-unstyled">
     <li class="page-design"><NuxtLink to="/">Home page</NuxtLink></li>
      <li class="page-design"><NuxtLink to="/dashboard">Dashboard</NuxtLink></li>
       <li class="page-design"> <NuxtLink to="/form">Form</NuxtLink></li>
        <li class="page-design">  <NuxtLink to="/table">Table</NuxtLink></li>
           <li class="page-design"> <NuxtLink to="/Modal">Modal</NuxtLink></li>
              <li class="page-design"> <NuxtLink to="/wizard">Wizard</NuxtLink></li>
               <li class="page-design"> <NuxtLink to="/Webpage">Web-Page</NuxtLink></li>
                 <li class="page-design"> <NuxtLink to="/login">Login</NuxtLink></li>
   </ul>
   </div>
  <Tutorial/>
 
</div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style scoped>
 ul, dl {
    margin-top: 0;
     margin-bottom:6px !important;
 }
.navbar{
  background-color: rgb(245, 245, 245);
}
ul li {
  margin-top: 10px;
 background-color:rgb(49, 158, 177);
  color: rgb(12, 11, 11) !important;
   padding: 0.25rem 0.6rem;
    line-height: 1.5;
    border-radius: 0.25rem;
     box-shadow: 0 7px 14px rgb(50 50 93 / 10%), 0 3px 6px rgb(0 0 0 / 8%);
    transform: translateY(-1px);
}
a {
 color: rgb(12, 11, 11) !important;
    text-decoration: none;
    background-color: transparent;
}
.page-design{
    display: inline-block;
  text-align:left;
  padding: 10px;
  text-decoration: none;
  font-size: 15px; 
  line-height: 25px;
  border-radius: 4px;
}
</style>
