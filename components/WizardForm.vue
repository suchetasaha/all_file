<template>
<div>
    <b-container fluid>
        <div class="wrapper">
            <div class="inner">
    <div class="form-content">
        <div class="registration">
        <h3>REGISTRATION</h3>
        </div>
    <form-wizard ref="wizard">
      <tab-content title="Personal details" icon="ti-user">
               <p class="content">Please fill with your details </p>
        <form @submit.prevent="nextStep">
            <div class="form-group">
         <div class="form-row">
<div class="form-holder">
<input type="text" placeholder="First Name" class="form-control">
</div>
<div class="form-holder">
<input type="text" placeholder="Last Name" class="form-control">
</div>
</div>
        <div class="form-row">
<div class="form-holder">
<input type="text" placeholder="Your Email" class="form-control">
</div>
<div class="form-holder">
<input type="text" placeholder="Phone Number" class="form-control">
</div>
</div>
<div class="form-row">
<div class="form-holder">
<input type="text" placeholder="Age" class="form-control">
</div>
<div class="form-holder" style="align-self: flex-end; transform: translateY(4px);">
<div class="checkbox-tick">
<label class="male">
<input type="radio" name="gender" value="male" checked=""> Male<br>
<span class="checkmark"></span>
</label>
<label class="female">
<input type="radio" name="gender" value="female"> Female<br>
<span class="checkmark"></span>
</label>
</div>
</div>
</div>
            </div>
      <b-form-group>
      <b-form-radio class="bottom-radio"> Nor again is there anyone who loves or pursues or desires to obtaini.
</b-form-radio>
    </b-form-group>
          <input type="submit" style="visibility: hidden" />
        </form>
      </tab-content>
      <tab-content title="Additional Info" icon="ti-settings">
            <p class="content">Please fill with additional information <p>
        <form @submit.prevent="nextStep">
             <div class="screen-body-item">
          <div class="app-form">
        <div class="app-form-group">
              <input class="form-control" placeholder="Address">
            </div>
          <div class="app-form-group">
              <input class="form-control" placeholder="City">
            </div>
            <div class="app-form-group">
              <input class="form-control" placeholder="Zip-Code">
            </div>
            <div class="app-form-group">
              <input class="form-control" placeholder="Your Country">
            </div>
          </div>
             </div>
          <input type="submit" style="visibility: hidden" />
        </form>
      </tab-content>
      <tab-content title="Last step" icon="ti-check">
        <p class="content">Send an optional message </p>
        <p class="message">Your message here!</p>
          <b-form-textarea
    id="textarea-rows"
  ></b-form-textarea>
      <b-form-group>
      <b-form-radio class="condition">Please accept term and conditions ?</b-form-radio>
    </b-form-group>
      </tab-content>
    </form-wizard>
    </div>
  </div>
  </div>
    </b-container>
</div>
</template>
<script>
export default {
    name:"wizard-form",
    data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
  methods: {
    nextStep() {
      this.$refs.wizard.nextTab();
    },
  },
}
</script>
<style scoped>
.container-fluid, .container-sm, .container-md, .container-lg, .container-xl {
    padding-right: 0px !important;
    padding-left: 0px !important;
}
.form-row .form-holder {
    width: 40%;
}
.message{
     color: #666 !important;
         font-size: 15px;
}
.condition{
    cursor: pointer;
    color: #999;
    font-size: 14px;
    line-height: 1.9;
    transform: translateY(-5px);
}
.form-group{
    margin-top: 35px;
}
.checkbox-tick label {
    cursor: pointer;
    display: inline-block;
    padding-left: 23px;
    position: relative;
     color: #666;
}
.bottom-radio{
        cursor: pointer;
    color: #999;
    font-size: 14px;
    line-height: 1.9;
    transform: translateY(-5px);
    margin-top: 35px;
}
.form-row {
    display: flex;
    margin-bottom: 18px;
    margin-left: 35px;
}
.form-row .form-holder {
    margin-right: 30px;
}
.form-control {
    height: 37px;
    border: none;
    border-bottom: 2px solid #e6e6e6;
    width: 100%;
    color: #666;
}
.registration{
text-align: center;
}
.content{
    margin-top: 16px;
    font-size: 20px;
    color: #6d7f52;
    text-align: center;
    margin-bottom: 26px;
}
.registration h3 {
    font-size: 22px;
    color: #453e79;
    text-transform: uppercase;
    letter-spacing: 7px;
    padding: 5px 15px;
    display: inline-block;
    border: 1px solid #dad8e4;
    margin-bottom: 75px;
}
.inner {
    width: 50%;
    display: flex;
    background: #fff;
    box-shadow: 0 0 5px 0 rgb(0 0 0 / 20%);
    -webkit-box-shadow: 0 0 5px 0 rgb(0 0 0 / 20%);
    -moz-box-shadow: 0 0 5px 0 rgba(0,0,0,.2);
    -ms-box-shadow: 0 0 5px 0 rgba(0,0,0,.2);
    -o-box-shadow: 0 0 5px 0 rgba(0,0,0,.2);
}
.wrapper {
    height: 100%;
    background: #f9f6f1;
    display: flex;
    align-items: center;
    justify-content: center;
}
.form-content {
    width: 100%;
    padding-top: 25px;
  margin-left: 35px;
   margin-right: 35px;
}
.screen-body-item {
  flex: 1;
  padding: 20px;
}
.app-form-group {
  margin-bottom: 15px;
}
.app-form-control {
  width: 100%;
  padding: 10px 0;
  background: none;
  border: none;
  border-bottom: 1px solid #666;
  color: #ddd;
  font-size: 14px;
  outline: none;
  transition: border-color .2s;
}
.form-control {
    height: 37px;
    border: none;
    border-bottom: 2px solid #e6e6e6;
    width: 100%;
    color: #666;
}
.form-control {
    display: block;
    width: 100%;
    height: calc(1.5em + 0.75rem + 2px);
    padding: 0px !important;
}
.app-form-control::placeholder {
  color: #666;
}
.vue-form-wizard.md .wizard-icon-circle {
    width: 20px !important;
    height: 20px !important;
    font-size: 24px !important;
        border-color: #6d7f52 !important;
}
.vue-form-wizard.md .wizard-navigation .wizard-progress-with-circle {
    position: relative;
    top: 15px !important;
    height: 3px !important;
}
.wizard-btn {
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    border-width: 2px;
    background-color: transparent;
    font-size: 14px;
    font-weight: 600;
    padding: 6px 12px;
    min-width: 140px;
    background-color: #6d7f52 !important;
    border-color:none !important;
    color: white;
}
</style>