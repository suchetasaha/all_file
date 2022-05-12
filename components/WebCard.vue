<template>
<b-container fluid>
    <div class="card-box">
        <b-container>
            <div class="center-box">
                <b-row>
                    <b-col cols="4">
                        <div class="box">
                            <img src="img/img1.png">
                        <h5>Lorem ipsum dolor sit amet</h5>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores doloribus voluptatum dignissimos.</p>
                        
                        </div>
                    </b-col>
                     <b-col cols="4">
                          <div class="box">
                            <img src="img/img2.png">
                      <h5>Lorem ipsum dolor sit amet</h5>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores doloribus voluptatum dignissimos.</p>
                        
                        </div>
                     </b-col>
                      <b-col cols="4">
                           <div class="box">
                            <img src="img/img3.png">
                     <h5>Lorem ipsum dolor sit amet</h5>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores doloribus voluptatum dignissimos.</p>
                        
                        </div>
                      </b-col>
                </b-row>
            </div>
        </b-container>
    </div>
</b-container>
</template>
<script>
export default {
name:'card-file'
}
</script>
<style scoped>
.container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    width: 100%;
   padding-right: 0 !important;
   padding-left: 0 !important;
    }
.card-box{
    background-color: rgb(235, 233, 233);
}
.box img{
    height:100%;
    width: 100%;
}
.center-box{
    padding-top: 70px;
}
</style>