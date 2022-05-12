<template>
    <div>
        <b-container class="bv-example-row">
            <div class="travel">
             <b-row>
                 <b-col cols="5">
        <h1 class="travel-text">Travel to your dream destination</h1>
        <p class="travel-para">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iure minus ad laboriosam quae. laboriosam amet culpa at voluptas facere quae a.</p>
    <b-button class="reserve">Reserve Ticket</b-button>
                 </b-col>
                 <b-col cols="7">
                     <img src="https://wallpaperaccess.com/full/378016.jpg" class="mountain">
                 </b-col>
             </b-row>
            </div>
        </b-container>
          <WebMemory/>
          <WebCard/>
          <WebPlace/>
    </div>
</template>
<script>
export default{
    name:'home-page'
}
</script>
<style scoped>
.reserve{
    background-color: black;
    color:white;
    border:none;
  padding: 7px 22px;
  margin-top: 15px ;

}
.travel{
    margin-top: 40px;
      margin-bottom: 35px;
  
}
.mountain{
    width:100%;
    height:100%;
}
.travel-text{
    font-size: 50px;
}
.travel-para{
    font-size: 15px;
    margin-top: 10px;
}
</style>
