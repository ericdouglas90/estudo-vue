<template>
  <div>
    <table border="1">
      <tr>
        <th>Nome</th>
        <th>Completa</th>
      </tr>
      <tr v-for="(task, index) in tasks"  :key="index">
        <td>{{task.name}}</td>
        <td>{{task.completed}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default{
  data() {
    return {
      tasks: [
        {name: 'Lavar Louça', completed: true},
        {name: 'Lavar Carro', completed: false},
        {name: 'Lavar Banheiro', completed: true},
        {name: 'Lavar Copos', completed: false},
      ]
    }    
  }  
}
</script>

<style scoped>
  div {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  table {
    width: 500px;
  }
</style>