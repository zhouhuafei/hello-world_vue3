<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div style="text-align: center;">
      <div>
        <div>radio1：{{ formFields.radio1 }}</div>
        <div>
          <label><input type="radio" name="radio" value="radio1-1" v-model="formFields.radio1" />radio1-1</label>
          <label><input type="radio" name="radio" value="radio1-2" v-model="formFields.radio1" />radio1-2</label>
          <label><input type="radio" name="radio" value="radio1-3" v-model="formFields.radio1" />radio1-3</label>
        </div>
      </div>
      <div>
        <div>checkbox1：{{ formFields.checkbox1 }}</div>
        <div>
          <input type="checkbox" v-model="formFields.checkbox1" />
        </div>
      </div>
      <div>
        <div>checkbox2：{{ formFields.checkbox2 }}</div>
        <div>
          <label><input type="checkbox" value="checkbox2-1" v-model="formFields.checkbox2" />checkbox2-1</label>
          <label><input type="checkbox" value="checkbox2-2" v-model="formFields.checkbox2" />checkbox2-2</label>
          <label><input type="checkbox" value="checkbox2-3" v-model="formFields.checkbox2" />checkbox2-3</label>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { reactive } from 'vue'

const formFields = reactive({
  radio1: '1-1',
  checkbox1: true,
  checkbox2: []
})
</script>

<style scoped lang="scss">
input {
  margin: 5px;
}
</style>
