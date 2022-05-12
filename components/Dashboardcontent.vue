<template>
    <div>
        <div class="background">
          <Dashboardheader/>
        <Sale/>
        <DashboardList/>
        <DashboardPage/>
        <DashboardOrder/>
        <Footer/>
        </div>
    </div>
</template>
<script>
export default {
    name:"dashboard-files",
}
</script>
<style scoped>
.background{
   background: #141e30 !important;
}
</style>