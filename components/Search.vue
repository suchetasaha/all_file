<template>
<div>
   <div id="main" class="search-table">
  <label>
    Filter: 
    <input type="text" v-model="search"/>
  </label>
  <div v-for="customer in filteredCustomers">
   <span>{{customer.firstName}} {{customer.lastName}}</span>
  </div>
</div>
</div>
</template>
<script>
export default {
    name:"search-file",
data: function(){
        return {
        search: '',
        customers: [{
            "firstName": "Madd",
            "lastName": "Max",
          }, {
            "firstName": "Mark",
            "lastName": "Johnson",
          }, {
            "firstName": "Ron",
            "lastName": "Moor",
          },
        ]};
},
computed: {
    filteredCustomers() {
    	 var self = this;
       return this.customers.filter((cust) => {
         return cust.firstName.toLowerCase().indexOf(self.search.toLowerCase()) >= 0 ||                                       
           cust.lastName.toLowerCase().indexOf(self.search.toLowerCase()) >= 0;
       });
    }
}
}
</script>
<style scoped>
.search-table{
    margin-top: 20px;
}
</style>