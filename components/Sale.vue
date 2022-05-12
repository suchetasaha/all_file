<template>
    <div>
        <b-container>
            <div class="sale-progress">
                <b-row class="progress-div">
                    <b-col cols="3" class="sale-div">
                        <b-card class=" card-icon-bg card-icon-bg-primary o-hidden mb-20 text-center">
                       <b-card-body class="body-padding">
                             
                                <b-icon icon="person-fill" class="icon" aria-hidden="true"></b-icon>
                                <div class="content">
                                    <p class="text-muted mt-2 mb-0">New Leads</p>
                                    <p class="text icon-text text-24 line-height-1 mb-2">205</p>
                                    </div>
                       </b-card-body>
                        </b-card>
                    </b-col>
                     <b-col cols="3">
                         <b-card class="body-card card-icon-bg card-icon-bg-primary o-hidden mb-20 text-center">
                    <b-card-body class="body-padding">
                            
                             <b-icon icon="text-right" class="icon" aria-hidden="true"></b-icon>
                                <div class="content">
                                    <p class="text-muted mt-2 mb-0">Sales</p>
                                    <p class="text text-24 line-height-1 mb-2">$2205</p>
                                    </div>
                    </b-card-body>
                         </b-card>
                     </b-col>
                      <b-col cols="3">
                          <b-card class="body-card card-icon-bg card-icon-bg-primary o-hidden mb-20 text-center">
                        <b-card-body class="body-padding">
                        
                               <b-icon icon="shield-shaded"  class="icon" aria-hidden="true"></b-icon>
                                <div class="content">
                                    <p class="text-muted mt-2 mb-0">Oders</p>
                                    <p class="text text-24 line-height-1 mb-2">250</p>
                                    </div>
                        </b-card-body>
                          </b-card>
                      </b-col>
                       <b-col cols="3">
                           <b-card class="body-card card-icon-bg card-icon-bg-primary o-hidden mb-20 text-center">
                        <b-card-body class="body-padding">
                     
                              <b-icon icon="file-earmark-text"  class="icon" aria-hidden="true"></b-icon>
                                <div class="content">
                                    <p class="text-muted mt-2 mb-0">Expenses</p>
                                    <p class="text text-24 line-height-1 mb-2">$4205</p>
                                    </div>
                        </b-card-body>
                           </b-card>
                       </b-col>
                </b-row>
            </div>
        </b-container>
    </div>
</template>
<script>
export default {
name: "year-sale",
}
</script>
<style scoped>
.icon{
    font-size: 2.5rem;
    font-weight: 400;
    color:#141e30 !important;
        margin-top: 15px;
        margin-left: 15px;
}
.body-padding{
    padding:10px 8px!important;
    display: flex !important;
}
.card-body {
    flex: 1 1 auto;
    min-height: 1px;
     padding:5px 8px!important;
}
.sale-progress{
    margin-top: 30px;
}
.o-hidden {
    overflow: hidden;
}
.mb-30 {
    margin-bottom: 30px!important;
}
.card-icon-bg {
    position: relative;
    z-index: 1;
}
.card {
    border-radius: 10px;
    -webkit-box-shadow: 0 4px 20px 1px rgb(0 0 0 / 6%), 0 1px 4px rgb(0 0 0 / 8%);
    box-shadow: 0 4px 20px 1px rgb(0 0 0 / 6%), 0 1px 4px rgb(0 0 0 / 8%);
    border: 0;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-color: #fff;
    background-clip: border-box;
}
.card-icon-bg .card-body .content {
    margin: auto !important;
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
    -webkit-box-align: start !important;
    -ms-flex-align: start !important;
    align-items: flex-start !important;
}

.text-muted {
    color: #4b5563!important;
}
.text{
     color: rgb(27, 27, 73)!important;
     font-size: 24px !important;
         font-size: 20px !important;
}
.card-icon-bg .card-body, .card-icon-bg .card-body .content {
    display: flex !important;
}
@media (max-width: 800px){
    .card-body {
    padding: 5px 4px!important;
    }
}
  @media (max-width: 640px){
      .icon {
    font-size: 1.7rem;
     margin-left: 0px;
      }
       .icon-text {
    margin-left: 10px;
   }
       .body-card{
        padding:12px 2px !important;
    }
  } 
    @media (max-width: 460px){
.text {
    color: rgb(27, 27, 73)!important;
    font-size: 20px !important;
    font-size: 17px !important;
}
     .icon {
    font-size: 1.2rem;
     margin-left: 0px;
      }
    }
 @media screen and (min-device-width: 320px) and (max-device-width: 640px) { 
      .progress-div{
          flex-direction: column;
      }
 }
@media screen and (min-device-width: 320px) and (max-device-width: 480px) { 
      .icon {
    font-size: 2.5rem;
    font-weight: 400;
    color: #141e30 !important;
    margin-top: 7px;
      }
            .sale-div{
          max-width: 100%;

      }
 }
</style>