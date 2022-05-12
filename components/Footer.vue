<template>
<div>
    <b-container fluid>
      <div class="footer">
        <section id="fooview" class="d-flex align-items-center">
          <div class=" container d-flex justify-content-center justify-content-md-between">
            <p class="copyright quick-links">
              Copyright © 2019 <span style="color: #141e30">Septiandika Pratama</span>.All Right Reserved
            </p>
            <div class="contact-info d-flex align-items-center">
              <span>Version 2.0.0
              </span>
            </div>
          </div>
        </section>
      </div>
    </b-container>
</div>
</template>
<script>
export default {
    name:"footer-page",
}
</script>
<style scoped>
.container, .container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    width: 100%;
     padding-right: 0px !important;
     padding-left: 0px !important;
    margin-right: auto;
    margin-left: auto;
}
.footer {
    background-color: white;
    padding-top: 15px;
    box-shadow: 0 -5px 5px -7px #333;
    margin-top: 15px;
}
.copyright {
    font-size: 14px;
    font-weight: 700;
    color: #727171;
}
.contact-info {
    font-size: 13px;
    font-weight: 700;
    color: #727171;
}
  @media (max-width: 580px){
.copyright{
  margin-bottom: -1px;
}
.contact-info{
  margin-left: 20px;
}
  }
</style>