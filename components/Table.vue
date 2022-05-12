<template>
<div>
    <div>
    <b-container>
        <div class="md-toolbar-section-start">
          <h3 class="md-title">Users</h3>
        </div>
    <div class="table" v-if="!hide">
        <div>
           <!--  <div v-for="item in filteredCustomers">
   <span>{{item.firstName}} {{item.lastName}}</span>
  </div>-->
<table v-if="name">
    <thead>
        <tr>
            <th>User</th>
              <th>Department</th>
                <th>employee</th>
               
        </tr>
    </thead>
    <tbody>
        <tr v-for="(row, index) in filteredCustomers" :key="`employee-${index}`">
            <td v-html="(row.user)"></td>
              <td v-html="(row.department)"></td>
                  <td v-html="([...row.employees].sort().join(', '))"></td>
        </tr>
    </tbody>
</table>
  </div>
    </div>
     <b-button @click="hideTable" class="hide">Hide</b-button>
    </b-container>
</div>
<Search/>
<SecondSearch/>
</div>
</template>
<script>
export default {
    name:'table-design',
    data() {
        
      return {
                search: '',
           hide:false,
        // Note 'isActive' is left out and will not appear in the rendered table
        rows: [{
                    user: 'Rahul',
                    department: 'Accounting',
                    employees: ['Bradley', 'Jones', 'Alvarado']
                },
                {
                    user: 'Rohit',
                    department: 'Human Resources',
                    employees: ['Juarez', 'Banks', 'Smith']
                },
                {
                    user: 'Virat',
                    department: 'Production',
                    employees: ['Sweeney', 'Bartlett', 'Singh']
                },
                {
                    user: 'Dhoni',
                    department: 'Research ',
                    employees: ['Lambert', 'Williamson', 'Smith']
                },
                {
                    user: 'Jadeja',
                    department: 'Sales and Marketing',
                    employees: ['Prince', 'Townsend', 'Jones']
                }
            ]
      }
    },
    
        methods: {
                 hideTable(){
            this.hide=!this.hide
        },
        
    },
    computed: {
     filteredCustomers() {
            return this.rows.filter(row => {
                const user = row.user.toLowerCase();
                const employees = row.employees.toString().toLowerCase();
                const department = row.department.toLowerCase();
                const searchTerm = this.search.toLowerCase();

                return user.includes(searchTerm) || department.includes(searchTerm) ||
                    employees.includes(searchTerm);
            });
        }
}
}
</script>
<style scoped>
.table{
    margin-top: 20px;
}
.hide{
    background-color: dimgrey;
    color:white;
    padding:6px 40px;
    border-radius: 8px;
}
</style>