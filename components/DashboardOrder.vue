<template>
    <div>
        <b-container>
            <div class="order">
        <b-row>
            <b-col cols="12">
                <b-card class=" mb-30">
                    <b-card-body class="p-0">
                   <h5 class="card-title p-3 mb-2">Recent Order</h5>
                   <div class="wrap">
                       <div class="inner-wrap">
                            <div>
    <b-table striped hover :items="items" :fields="fields"></b-table>
  </div>
                       </div>
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
    name:"recent-order",
    data() {
      return {
        // Note 'isActive' is left out and will not appear in the rendered table
        fields: [
             {
            key: 'Order_Id',
               label: 'Order_Id',
            sortable: true
          },
          {
            key: 'Buyer_Name',
               label: 'Buyer_Name',
            sortable: true
          },
          {
            key: 'Product',
               label: 'Product',
            tdClass: 'table-style',
            sortable: false
          },
          {
            key: 'Status',
               label: 'Status',
            tdClass: 'status',
            sortable: false
          },
          {
            key: 'Shpping_Cost',
               label: 'Shpping_Cost',
            tdClass: 'table-style',
            sortable: false
          },
          {
            key: 'Date',
               label: 'Date',
            tdClass: 'table-style',
            sortable: false
          },
          {
            key: 'Action',
            tdClass: 'view-style',
            label: 'Action',
            sortable: true
          }
        ],
        items: [
          { isActive: true, Action: 'View', Date: '31st 19', Shpping_Cost: '3.5%',Status: 'Delivered',Product: 'Carney', Buyer_Name: 'Carney',Order_Id: 1,},
          { isActive: false, Action:'View', Date: '31st 11', Shpping_Cost: '6.2%',Status: 'Shppied',Product: 'Carney',Buyer_Name: 'Jone',Order_Id: 2, },
          { isActive: false, Action: 'View', Date: '31st 19', Shpping_Cost: '3.2%',Status: 'Delivered',Product: 'Carney', Buyer_Name: 'jane', Order_Id: 3,},
          { isActive: true, Action: 'View', Date: '31st 11', Shpping_Cost: '3.34%',Status: 'Pending',Product: 'Carney',Buyer_Name: 'Susan', Order_Id: 4,},
          { isActive: true, Action: 'View', Date: '31st 19', Shpping_Cost: '3.34%',Status: 'Processing',Product: 'Carney',Buyer_Name: 'Carney',Order_Id: 5, }

        ]
      }
    }
}
</script>
<style scoped>
.order{
    margin-top: 15px;
}
.table th, .table td {
    padding: 0.75rem;
    vertical-align: top;
    border-top: none !important; 
    font-size: 14px !important;
}
.card-title {
    font-size: 1.1rem
}
.status{
background: unset;
    border: 1px solid #8b5cf6;
    color: #8b5cf6;
    font-weight: 600;
    padding: 0.5rem!important;
    border-radius: 10rem;
}
@media (max-width: 800px){
  .inner-wrap{
      overflow-x: scroll;
  }
}

</style>