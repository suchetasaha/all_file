<template>
    <div>
        <b-container>
            <div class="table-box">
            <b-row class="page-div">
                <b-col cols="8" class="table-div">
                    <div>
                       <b-card>
                <div class="table-one align-items-center">
                    <b-row >
                    <b-col>
                        <h3 class="mb-0 page">Page visits</h3>
                    </b-col>
                 <b-col class="text-right">
                     <a href="#!" class="btn btn-sm btn-primary">See all</a>
                 </b-col>
                    </b-row>
                    <div class="page-card table-div">
                     <b-table striped hover :items="items" :fields="fields"></b-table>
                    </div>
                 </div>
                 
            </b-card>
                    </div>
                </b-col>
                <b-col cols="4" class="table-div">
                  <div class="table-two">
                      <b-card>
                          <b-card-header>
                          <h5 class="mb-0 progress-header">Progress Track</h5>
                          </b-card-header>
                          <b-card-body>
                              <b-list-group>
  <b-list-group-item>
      <b-row>
          <b-col>
              <img alt="Image placeholder" class="bootstrap" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARMAAAC3CAMAAAAGjUrGAAAAe1BMVEX///9WPXxPM3dMMHaglrO2rsRTOHpCH29VO3taQn9zYpFGJnLj4OhwXY5KLHRDIXD08/Z9bZilm7ZJKnPNyNa+t8rY1N+qobqDdJyJe6GZjq1fSILy8fTKxNPUz9yek7Hq6O7b2OI9F2yUh6ljTYVxX4/Dvc+xqcBoU4gxSCJUAAAESklEQVR4nO2da5eqIBSGvYxiYlipXWbsNs3U+f+/8NjM+YBKQmeVpPt9PrNY8SwI2G7AcQAAAAAAAAAAAAAAAAAAAAAAAAAAbJDkRfB4ijyx3bD/pAzilAvhPx4heBoHpe0G3k2yZn7oPo/QZ+th9ZbZhj1TyD8tbDOz3VBz8sx7upErXpbbbqopK9aLkStsZbuxZrzz3pS4Ln+33VwTFn0qqaQsbDdYz7a/gfML29puso4Zj3p2EvFXn33mz5+Dm4Rz243uZpn2rsR106XtZnfy3X83qTrKt+1md5HY6CZVR3nlVf6in/VrE++V5+OPviedX6IP2w2/zczO0KkGz+tOx7vMkpNsZ7vpNyl8S078wnbTb7Ky5uR1t8dvdqadauJ5s930m8BJGzhpAydt4KQNnLTROvGYlpSlPBN+eNcuYcBODPdqZZKv1hn3zLUM2ck9P/24F8LUChUnFYFnuDAm5MRx9syoq5By4iyFSTSTlhOnNJmBiDlxSoOgDDUnTq7/2ErOibPW/qXQc3LQhnlH4ySeKojXb9tWwDnWdZTROHFDJZ5gm0b+3llQcTK5Ocl6jfyJUjd4CDhxo89jrWLtfpuAEzea1CrWZXCQcOLyWv7E6TkTWh880Ek91PKkSb4PHuiknnyky1eg4ST6kovCyY+TSC6K/5MfJ65cFPPOlXAqF8X65KfoSSp50EULaDgRZ6lkoAtV03CSySW1aXIknHA58WirjT5ScJJt5IKuNko9fich28vlNvov86Nxoo4peX76XQsUXAzOA43GSaxifgoOtTovJjm3o3FixMno1BglJ8uJ2Ud0Ok5200/Doy90nMx2e88sBYWOkytno9FDy4njLAwOolJz4iwzOutYYxLt+dzROEnUHNrnk5a64TMaJz5Xk3qbc7NizR/taJzc3heHIgvqNUfdo4eAk4osrtWsySyg4cT1akFqTZSaiBNXrMyrpuLEZfIEdOyMP5Jx4tf+ZztjBmSc1D+jd+a0kXESCbn0e1fdZJy4qVz60rVso+OkdilQ5wqFqJMtnFxhcmk4uVK/1QRj56e0nG7RnVtAxgnfGddNxUnjQqDO9C0qThrp5Z1BWSJO2KVW9RH7nfCzcRvQnnasIAp9Nj80qu7+HjgaJyJVhqj9r037TvLO3c6InNzBTPPZi6ITMnnU5izInAc0Rp/RRs6JwT3oxJwcprqBQ87JwuiRCUJOykWGHD+ZsoiZ6TVTQ3ZieEfyYVmcPlKjG3IG7yT6UuZOy0z/THjKM/+Oi8iG7aTa3mmJNKkmo3PyLOAETgbuBPdRt8G95W1wv30bvIOgAO9ltMG7Km3w/o4CvNPUBu95KcC7b23wPqACvCOpAO+NKsC7tArwfrECvHOtAO+hq0jWzH+mltBn65de0SspgzjlQviPRwiexu1cpoGQ5EXweIp8eD0EAAAAAAAAAAAAAAAAAAAAAAAAAOPgLzAmXvPHw9xoAAAAAElFTkSuQmCC">
          </b-col>
          <b-col>
              <h5 class="design">Design System</h5>
              <div class="progress-system">
  <span class="progress-bar" style="width: 75%"></span>
</div>
          </b-col>
      </b-row>
  </b-list-group-item>
  <b-list-group-item>
      <b-row>
          <b-col>
               <img class="bootstrap" src="data:image/png;base64,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" alt="user" width="50">
                    
          </b-col>
          <b-col> 
<h5 class="design">Angular Design</h5>
<div class="progress-system">
  <span class="progress-bar" style="width: 75%"></span>
</div>
          </b-col>
      </b-row>
  </b-list-group-item>
  <b-list-group-item>
      <b-row>
          <b-col>
               <img class="bootstrap" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQI0RAllozh2bKCwPOYa6fqlTm7nSkGG_rFvQ1PKbMyOFqbySD76m6wslx1zryADjqgj_E&usqp=CAU" alt="user" width="50">
                     
          </b-col>
          <b-col>
              <h5 class="design">React Material</h5>
              <div class="progress-system">
  <span class="progress-bar" style="width: 75%"></span>
</div>
          </b-col>
      </b-row>
  </b-list-group-item>
</b-list-group>
                          </b-card-body>
                      </b-card>
                  </div>
                </b-col>

            </b-row>
            </div>
        </b-container>
    </div>
</template>
<script>
export default {
    name:"page-visit",
    data() {
      return {
        // Note 'isActive' is left out and will not appear in the rendered table
        fields: [
          {
            key: 'last_name',
            sortable: true
          },
          {
            key: 'first_name',
            sortable: false
          },
          {
            key: 'age',
            label: 'Person age',
            sortable: true,
            // Variant applies to the whole column, including the header and footer
            variant: 'danger'
          }
        ],
        items: [
          { isActive: true, age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { isActive: false, age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { isActive: false, age: 89, first_name: 'Geneva', last_name: 'Wilson' },
          { isActive: true, age: 38, first_name: 'Jami', last_name: 'Carney' }
        ]
      }
    }
}
</script>
<style scoped>

.progress-system{
  width: 100%;
  max-width: 290px;
  height: 3px;
  background: #e1e4e8;
  border-radius: 3px;
  overflow: hidden;
  }
  .progress-bar{
    display: block;
    height: 100%;
        background-color: #254074!important;
    background-size: 300% 100%;
    animation: progress-animation 2s linear infinite;
    }
.bootstrap{
    width: 100%;
    height: 100%;
          color: #fff;
    background-color: #adb5bd;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    font-size: 1rem;
    height: 48px;
    width: 48px;
}
.design{
    font-size: .8125rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 600;
    line-height: 1.5;
    color: #32325d
}
.list-group-item {
    position: relative;
    display: block;
    padding: 0.75rem 1.0rem !important;
    background-color: #fff;
    border-width: 0 0 1px;
}
.progress-header{
    font-family: inherit;
    font-weight: 600;
    line-height: 1.5;
    color: #141e30;
        font-size: 1.0625rem;
}
.table-box{
    margin-top: 19px;
}
.table-div{
    margin-top: 13px;
}
.btn-primary, .btn-primary:hover {
    color: #fff;
    background-color: #141e30;
    border-color: #141e30;
}
.btn-primary {
    box-shadow: 0 4px 6px rgb(50 50 93 / 11%), 0 1px 3px rgb(0 0 0 / 8%);
}
.btn {
    position: relative;
    text-transform: none;
    transition: all .15s ease;
    letter-spacing: .025em;
    font-size: .875rem;
    will-change: transform;
}

.btn-group-sm>.btn, .btn-sm {
    padding: 0.25rem 0.5rem;
    line-height: 1.5;
    border-radius: 0.25rem;
}
.page {
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 600;
    line-height: 1.5;
    color: #141e30;
        font-size: 1.0625rem;
}
table td {
    font-size: 14px;
    padding: 0.75rem;
    vertical-align: top;
    border-top: 1px solid #dee2e6;
}
.card-body {
    flex: 1 1 auto;
    min-height: 1px;
    padding: 1.2rem !important;
}
@media (max-width: 1024px){
.table-one{
    padding-bottom: 10px;
}
}
@media (max-width: 800px){
    .table-one {
    padding-bottom: 90px;
    }
}
@media (max-width: 460px){
    .page-card{
          overflow-x: scroll;
    }
    .card-body {
    flex: 1 1 auto;
    min-height: 1px;
     padding: 0px !important;
    }
    .table-one {
    padding-bottom: 75px;
    }
}
@media screen and (min-device-width: 320px) and (max-device-width: 640px) { 
    .page-div{
        flex-direction: column;
    }
    .table-div{
        max-width:100%;
    }
}
</style>