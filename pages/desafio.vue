<template>
    <div id="app">
        <v-app id="inspire">
            <v-row>
                <v-col cols="4" v-for="(personaje,i) in this.personajes" :key="i">
                    <v-card
                    class="m-auto"
                    max-width="300"
                    >
                    <v-img :src="personaje.imagen">
                    </v-img>
                
                    <v-card-title>
                        {{personaje.nombre}}
                    </v-card-title>
                    </v-card> 
                </v-col> 
            </v-row>         
        </v-app>
    </div>
</template>
<script>
export default {
  data() {
    return {
      personajes: [
        {
          id: 1,
          nombre: "Morty",
          imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"
        },
        {
          id: 2,
          nombre: "Rick",
          imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"
        },
        {
          id: 3,
          nombre: "Summer",
          imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"
        },
        {
          id: 4,
          nombre: "Beth",
          imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"
        },
        {
          id: 5,
          nombre: "Jerry",
          imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"
        }
      ]
    };
  }
};
</script>
