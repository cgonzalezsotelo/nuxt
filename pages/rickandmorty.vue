<template>
  <main>
    <v-row>
      <v-col v-for="(personaje, index) in personajes" :key="index">
        <v-card>
          <v-img height="250" :src="personaje.imagen"></v-img>

          <v-card-title>{{ personaje.nombre }}</v-card-title>

          <v-divider class="mx-4"></v-divider>
        </v-card>
      </v-col>
    </v-row>
  </main>
</template>
<script>
export default {
  data: () => ({
    personajes: [
      {
        id: 1,
        nombre: 'Morty',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
      },
      {
        id: 2,
        nombre: 'Rick',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
      },
      {
        id: 3,
        nombre: 'Summer',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
      },
      {
        id: 4,
        nombre: 'Beth',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
      },
      {
        id: 5,
        nombre: 'Jerry',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
      },
    ],
  }),
}
</script>
