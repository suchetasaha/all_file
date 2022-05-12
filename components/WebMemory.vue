<template>
 <b-container fluid>
    <div class="memory">
        <b-container>
        <div class="memory-center">
        <h3 class="memory-text">
            <span>Create a memory to remember</span></h3>
        <p class="memory-para">
            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores distinctio temporibus,</span><span> impedit vitae veritatis illo nam.
            </span>
            </p>
        <b-button class="travel">My TravelBlogs</b-button>
        </div>
        </b-container>
        </div>
 </b-container>
</template>
<script>
export default {
name: 'memory-file'
}
</script>
<style scoped>
.container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    width: 100%;
   padding-right: 0 !important;
   padding-left: 0 !important;
    }
.memory{
    background-color: black;
    margin-top: 10px;
    padding-bottom: 55px;
}
.memory-center{
    text-align: center;
  padding-top: 35px;
  color: white;
}
.memory-para{
    text-align: center;
    font-size: 15px;
    font-weight: 400;
    padding-right: 20px;
}
.memory-para{
    display: block;
}
.travel{
    background-color: transparent;
    border:2px solid white;
    color:white;
    padding:5px 25px;
}
</style>