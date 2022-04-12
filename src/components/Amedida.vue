<template>
  <div>
    <h1>Componente de Boostrap Tabla</h1>

    <table class="table">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Nombre</th>
          <th scope="col">Apellido</th>
          <th scope="col">RUT</th>
          <th scope="col">Nacimiento</th>
          <th scope="col">Edad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(persona, i) in listapersonas" :key="i">
          <th scope="row">{{ i + 1 }}</th>
          <td>{{ persona.nombre }}</td>
          <td>{{ persona.apellido }}</td>
          <td>{{ persona.rut }}</td>
          <td>{{ persona.nacimiento }}</td>
          <td>{{ persona.edad }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "aMedida",

  data() {
    return {
      listapersonas: [
        {
          nombre: "jose",
          apellido: "perez",
          rut: "123456-2",
          nacimiento: "12-04-67",
          edad: 52,
        },
        {
          nombre: "María",
          apellido: "Rodríguez",
          rut: "654321-1",
          nacimiento: "30-11-90",
          edad: 29,
        },
        {
          nombre: "Manuel",
          apellido: "Patiño",
          rut: "14223456-6",
          nacimiento: "02-12-59",
          edad: 60,
        },
      ],
    };
  },
};
</script>
