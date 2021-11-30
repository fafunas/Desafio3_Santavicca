<template>
  <div>
      <table :class="estilo">
        <tr>
          <td><p>Nombre</p></td>
          <td><p>Edad</p></td>
          <td><p>Sexo</p></td>
          <td><p>Nacionalidad</p></td>
        </tr>
        <tr v-for="(persona,i) in personas" :key="i">
          <td>{{persona.nombre}}</td>
          <td>{{persona.Edad}}</td>
          <td>{{persona.Sexo}}</td>
          <td>{{persona.Nacionalidad}}</td>
        </tr>
      </table>
    </div>
</template>

<script>
export default {};
</script>

<style>
.list-even tr:nth-child(even) {
    background-color: #D6EEEE;
}

.list-odd tr:nth-child(odd) {
    background-color: #D6EEEE;
}


table{
    width: 100%;
    padding-top: 10px;
    margin-top: 10px;
}
</style>