<template>
  <v-data-table :class="estilo"
    :headers="headers"
    :items="items"
    :items-per-page="5"
    hide-defaul-footer
  ></v-data-table>
</template>

<script>
export default {
  props: {
    personas: Array,
    estilo: String,
  },
  data() {
    return {
      headers: [
        {
          align: "start",
          sortable: false,
          value: "name",
        },
        { text: "Nombre", value: "nombre" },
        { text: "Edad", value: "Edad" },
        { text: "Sexo", value: "Sexo" },
        { text: "Nacionalidad", value: "Nacionalidad" },
      ],
      items: [
        {
          nombre: "Fabian",
          Edad: 34,
          Sexo: "Masculino",
          Nacionalidad: "Argentino",
        },
        {
          nombre: "Maria",
          Edad: 30,
          Sexo: "Femenino",
          Nacionalidad: "Argentina",
        },
        {
          nombre: "Juan",
          Edad: 50,
          Sexo: "Masculino",
          Nacionalidad: "Paraguayo",
        },
        {
          nombre: "Silvia",
          Edad: 25,
          Sexo: "Femenino",
          Nacionalidad: "Chilena",
        },
      ],
    };
  },
};
</script>

<style>
.list-even tr:nth-child(even) {
  background-color: #d6eeee;
}

.list-odd tr:nth-child(odd) {
  background-color: #d6eeee;
}

table {
  width: 100%;
  padding-top: 10px;
  margin-top: 10px;
}
</style>