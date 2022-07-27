<template>
    <v-container id="skillsContainer">

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="html"
            >
            </v-sheet>
            <h3 class="techName">HTML</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="css"
            >
            </v-sheet>
            <h3 class="techName">CSS</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="javaScript"
            >
            </v-sheet>
            <h3 class="techName">JavaScript</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="vue"
            >
            </v-sheet>
            <h3 class="techName">Vue.js</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="python"
            >
            </v-sheet>
            <h3 class="techName">Python</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="flask"
            >
            </v-sheet>
            <h3 class="techName">Flask</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="pinia"
            >
            </v-sheet>
            <h3 class="techName">Pinia</h3>
        </div>

        <div class="techContainer">
            <v-sheet
            elevation="14"
            height="75px"
            width="75px"
            id="maria"
            >
            </v-sheet>
            <h3 class="techName">MariaDB</h3>
        </div>
      
  </v-container>
</template>

<script>
    export default {
        name: "TechnicalSkills",
        
    }
</script>

<style lang="scss" scoped>
#skillsContainer{
    display: grid;
    grid-template-rows: 1fr, 1fr;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    align-items: center;
    justify-items: center;
    .skillsHeader{
        position: absolute;
        justify-content: center;
        padding: px;
        top: 0vh;
    }
    .techContainer{
        display: grid;
        grid-template-rows: 2fr 1fr ;
        justify-items: center;
        .techName{
        position: relative;
        grid-row: 2;
        color: whitesmoke;
        }
        #html{
            position: relative;
            background: url('https://cdn-icons-png.flaticon.com/512/143/143655.png') ;
            background-size: cover;
            background-color: #343030;
            
        }
        #css{
            background: url('https://cdn-icons-png.flaticon.com/512/732/732190.png');
            background-size: cover;
            background-color: #343030;
        }
        #javaScript{
            background: url('https://cdn-icons-png.flaticon.com/512/5968/5968292.png');
            background-size: cover;
            background-color: #343030;
        }
        #vue{
            background: url('https://png2.cleanpng.com/sh/ccfdd8eb1c34f06bec4af7540a438038/L0KzQYm3VcI3N5JuiJH0aYP2gLBuTgZ2bV5vi59zYYbkg7T5igB1NZd3ed9ud3B1e37ukvFxcKJxReV4ZoT6ccPsTfZzaZ5qReY2dj24coGBhfRkO5Y2UKcDNj62RYe5UcUyPWI6Sqk8MUG7QYKCUsM5NqFzf3==/kisspng-vue-js-javascript-framework-graphql-software-frame-t-v-5b08edc3e18586.3562151515273118119238.png');
            background-size: cover;
            background-color: #343030;
        }
        #python{
            background: url('https://cdn-icons-png.flaticon.com/512/5968/5968350.png');
            background-size: cover;
            background-color: #343030;
        }
        #flask{
            background: url('https://brandeps.com/logo-download/F/Flask-logo-vector-01.svg');
            background-size: cover;
            background-color: #343030;
        }
        #pinia{
            background: url('https://miro.medium.com/max/700/1*TOGHpRhMF0wGXhsrCga94w.png') center;
            background-size: cover;
            background-color: #616a72;
        }
        #maria{
            background: url('https://mariadb.com/wp-content/uploads/2019/11/mariadb-logo-vertical_white.svg') no-repeat;
            width: 30%;
            background-color: #616a72;
        }
    }
    
}
</style>