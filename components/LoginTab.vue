<template>
    <div>
  <b-card no-body>
    <b-tabs card>
      <b-tab title="Tab 1" active>
     <div class="sign-up">
    <div class="form">
      <div class="subtitle">Fill Your Form</div>
      <div class="input-container ic1">
        <input
          id="firstname"
          class="input"
          type="text"
          placeholder=" "
          v-model="firstname"
        />

        <label for="firstname" class="placeholder">First name</label>
      </div>
      <div class="input-container ic2">
        <input
          id="lastname"
          class="input"
          type="text"
          placeholder=" "
          v-model="lastname"
        />
        <label for="lastname" class="placeholder">Last name</label>
      </div>
      <div class="input-container ic2">
        <input
          id="email"
          class="input"
          type="text"
          placeholder=" "
          v-model="email"
        />
        <label for="email" class="placeholder">Email</label>
      </div>
       <div class="input-container ic2">
        <input
          id="email"
          class="input"
          type="text"
          placeholder=" "
          v-model="password"
        />
        <label for="email" class="placeholder">password</label>
      </div>
      <button type="text" class="submit" @click="registerForm">Register</button>
    </div>
  </div>
      </b-tab>
      <b-tab title="Tab 2">
        <form method="POST" action="">
<div class="container">
    <div id="app">
        <step-navigation :steps="steps" :currentstep="currentstep">
        </step-navigation>
        
        <div v-show="currentstep == 1">
            <h1>Step 1</h1>
            <div class="form-group">
                <label for="email">Email address</label>
                <input type="email" name="email" class="form-control" aria-describedby="emailHelp" placeholder="Enter email">
                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
            </div>
            <div class="form-group">
                <label for="password">Password</label>
                <input type="password" name="password" class="form-control" placeholder="Password">
            </div>
        </div>

        <div v-show="currentstep == 2">
            <h1>Step 2</h1>
            <div class="form-group">
                <label for="select">Example select</label>
                <select class="form-control" name="select">
                    <option>1</option>
                    <option>2</option>
                    <option>3</option>
                    <option>4</option>
                    <option>5</option>
                </select>
            </div>
        </div>

        <div v-show="currentstep == 3">
            <h1>Step 3</h1>
            <div class="form-group">
                <label for="textarea">Example textarea</label>
                <textarea class="form-control" name="textarea" rows="4"></textarea>
            </div>
            <div class="form-group">
                <label for="file">File input</label>
                <input type="file" class="form-control-file" name="file" aria-describedby="fileHelp">
                <small id="fileHelp" class="form-text text-muted">This is some placeholder block-level help text for the above input. It's a bit lighter and easily wraps to a new line.</small>
            </div>
        </div>

        <step v-for="step in steps" :currentstep="currentstep" :key="step.id" :step="step" :stepcount="steps.length" @step-change="stepChanged">
        </step>

        <script type="x-template" id="step-navigation-template">
            <ol class="step-indicator">
                <li v-for="step in steps" is="step-navigation-step" :key="step.id" :step="step" :currentstep="currentstep">
                </li>
            </ol>
        </script>

        <script type="x-template" id="step-navigation-step-template">
            <li :class="indicatorclass">
                <div class="step"><i :class="step.icon_class"></i></div>
                <div class="caption hidden-xs hidden-sm">Step <span v-text="step.id"></span>: <span v-text="step.title"></span></div>
            </li>
        </script>

        <script type="x-template" id="step-template">
            <div class="step-wrapper" :class="stepWrapperClass">
                <button type="button" class="btn btn-primary" @click="lastStep" :disabled="firststep">
                    Back
                </button>
                <button type="button" class="btn btn-primary" @click="nextStep" :disabled="laststep">
                    Next
                </button>
                <button type="submit" class="btn btn-primary" v-if="laststep">
                    Submit
                </button>
            </div>
        </script>
    </div>
</div>
</form>
      </b-tab>
    </b-tabs>
  </b-card>
</div>
</template>
<script>
export default {
name:'tab-view'
}
</script>
<style scoped>

.sign-up {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.form {
  background-color: #c9c9ca;
  border-radius: 5px;
  box-sizing: border-box;
  height: 50%;
  padding: 20px;
  width: 60%;
  margin-top: 30px;
}

.subtitle {
  color: black;
  font-family: sans-serif;
  font-size: 18px;
  font-weight: 600;
  margin-top: 10px;
  text-align: center;
}

.input-container {
  height: 50px;
  position: relative;
  width: 100%;
}

.ic1 {
  margin-top: 40px;
}

.ic2 {
  margin-top: 30px;
}

.input {
  background-color: #dadadd;
  border-radius: 8px;
  border: 0;
  box-sizing: border-box;
  color: #eee;
  font-size: 18px;
  height: 100%;
  outline: 0;
  padding: 4px 20px 0;
  width: 100%;
}

.input:focus ~ .cut,
.input:not(:placeholder-shown) ~ .cut {
  transform: translateY(8px);
}

.placeholder {
  color: #65657b;
  font-family: sans-serif;
  left: 20px;
  line-height: 14px;
  pointer-events: none;
  position: absolute;
  transform-origin: 0 50%;
  transition: transform 200ms, color 200ms;
  top: 20px;
}

.input:focus ~ .placeholder,
.input:not(:placeholder-shown) ~ .placeholder {
  transform: translateY(-30px) translateX(10px) scale(0.75);
}

.input:not(:placeholder-shown) ~ .placeholder {
  color: #808097;
}

.input:focus ~ .placeholder {
  color: #dc2f55;
}

.submit {
  background-color: #08d;
  border-radius: 12px;
  border: 0;
  box-sizing: border-box;
  color: #eee;
  cursor: pointer;
  font-size: 18px;
  height: 50px;
  margin-top: 38px;
  text-align: center;
  width: 100%;
}

.submit:active {
  background-color: #06b;
}




</style>