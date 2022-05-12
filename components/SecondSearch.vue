<template>
<div>
    <div>
<b-card bg-variant="light">
    <b-form-group
      label-cols-lg="3"
      label="Shipping Address"
      label-size="lg"
      label-class="font-weight-bold pt-0"
      class="mb-0"
    >
      <b-form-group
        label="Street:"
        label-for="nested-street"
        label-cols-sm="3"
        label-align-sm="right"
      >
        <b-form-input id="nested-street"></b-form-input>
      </b-form-group>

      <b-form-group
        label="City:"
        label-for="nested-city"
        label-cols-sm="3"
        label-align-sm="right"
      >
        <b-form-input id="nested-city"></b-form-input>
      </b-form-group>

      <b-form-group
        label="State:"
        label-for="nested-state"
        label-cols-sm="3"
        label-align-sm="right"
      >
        <b-form-input id="nested-state"></b-form-input>
      </b-form-group>

      <b-form-group
        label="Country:"
        label-for="nested-country"
        label-cols-sm="3"
        label-align-sm="right"
      >
        <b-form-input id="nested-country"></b-form-input>
      </b-form-group>

      <b-form-group
        label="Ship via:"
        label-cols-sm="3"
        label-align-sm="right"
        class="mb-0"
        v-slot="{ ariaDescribedby }"
      >
        <b-form-radio-group
          class="pt-2"
          :options="['Air', 'Courier', 'Mail']"
          :aria-describedby="ariaDescribedby"
        ></b-form-radio-group>
      </b-form-group>
    </b-form-group>
     <div class="search-div">
    <!-- Styled -->
    <b-form-file
      v-model="file1"
      :state="Boolean(file1)"
      placeholder="Choose a file or drop it here..."
      drop-placeholder="Drop file here..."
    ></b-form-file>
    <div class="mt-3 right-portion">Selected file: {{ file1 ? file1.name : '' }}</div>

    <!-- Plain mode -->
    <b-form-file v-model="file2" class="mt-3" plain></b-form-file>
    <div class="mt-3">Selected file: {{ file2 ? file2.name : '' }}</div>
  </div>
  </b-card>
</div>
  </div>
</template>
<script>
export default {
    data() {
      return {
        file1: null,
        file2: null
      }
    }
}
</script>
<style scoped>
.custom-file {
    position: relative;
    display: inline-block;
    width: 60% !important;
    height: calc(1.5em + 0.75rem + 2px);
    margin-bottom: 0;
    left:40% !important;
    top:5% !important;
    bottom:0;
    margin-top: 10px;
}
input.is-invalid ~ .custom-file-label {
    border-color: #dc3545;
}
.search-div{
    position: relative;
}
.right-portion{
position:absolute;
  right: 50%;
  top:10%;
}
</style>