<template>
  <div id="app">
    <TesteComponent />
    <FormComponent />
    <hr>
    <TaskComponent />  
  </div>
</template>

<script>
import FormComponent from './components/FormComponent.vue';
import TaskComponent from './components/TaskComponent.vue';
import TesteComponent from './components/TesteComponent.vue';

export default {
  name: 'app',
  components: {
    TesteComponent,
    FormComponent,
    TaskComponent
},
  data () {
    return {
      msg: 'Curso de Vue JS'
    }
  },
 
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

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
