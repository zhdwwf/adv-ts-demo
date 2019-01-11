<template>
  <div id="app">
    <a-form :form="form">
      <a-form-item label="field">
        <a-input style="width:300px;margin:0 auto;" v-decorator="['name']"/>
      </a-form-item>
    </a-form>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from './components/HelloWorld.vue';

@Component({
  components: {
    HelloWorld,
  },
})
export default class App extends Vue {
  public form: any = this.$form.createForm(this);
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
