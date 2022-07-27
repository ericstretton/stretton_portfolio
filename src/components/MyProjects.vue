<template>
    <v-container>
        <v-subheader class="text-center justify-center py-6">
            <h3 class="font-weight-bold text-h3 font_color">
                My Projects
            </h3>
        </v-subheader>
        <v-container id="projectContainer">
            <v-card
                class="mx-auto cards"
                max-width="344"
                id="pizzaRicks"
            >
                <!-- <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
                ></v-img> -->

            <v-card-title
            class="cardText">
            Pizza Ricks
            </v-card-title>

            <v-card-subtitle
            class="cardText">
            Static Restaurant Site
            </v-card-subtitle>

            <v-card-actions>
            <v-btn
                color="orange lighten-2"
                text
                @click="navigatePizzaRicks()"
                class="gitLink"
            >
                Link to GitHub
            </v-btn>

            <v-spacer></v-spacer>

            <v-btn
                icon
                @click="show1 = !show1"
            >
            <v-icon>{{ show1 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
            </v-btn>
            </v-card-actions>

            <v-expand-transition>
            <div v-show="show1">
            <v-divider></v-divider>

            <v-card-text
            class="cardText">
            My first built website, I thorougly enjoyed being able to make something so unique! The website is static and uses only HTML and CSS. It gives a brief description of the restaurant, displays the menu and has a contact page.
            <p>Skills: HTML, CSS, SCSS, APACHE </p>
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>
        <v-card
                class="mx-auto cards"
                max-width="344"
                id="foodie"
            >
                <!-- <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
                ></v-img> -->

            <v-card-title
            class="cardText">
            Foodie
            </v-card-title>

            <v-card-subtitle
            class="cardText">
            Food Ordering App
            </v-card-subtitle>

            <v-card-actions>
            <v-btn
                color="orange lighten-2"
                text
                @click="navigateFoodieFe()"
                class="gitLink"
            >
                Link to FE GitHub 
            </v-btn>

            <v-btn
                color="orange lighten-2"
                text
                @click="navigateFoodieBe()"
                class="gitLink"
            >
                Link to BE GitHub 
            </v-btn>

            <v-spacer></v-spacer>

            <v-btn
                icon
                @click="show2 = !show2"
            >
            <v-icon>{{ show2 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
            </v-btn>
            </v-card-actions>

            <v-expand-transition>
            <div v-show="show2">
            <v-divider></v-divider>

            <v-card-text
            class="cardText">
            Foodie is a food ordering website based on some of the household food delivery app services. With Foodie you are able to sign up as user or a restaurant owner. 
            The owner can create their restaurant information for any users to interact and order with. I particularly enjoyed developing the API package for this and applying several useful regular expressions to work through accepting JSON data. 
            <p>Skills: HTML, CSS, SCSS, JavaScript, Vue.js, Python, Flask, Pinia, MariaDB, SQL, APACHE </p>
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>
        <v-card
                class="mx-auto cards"
                max-width="344"
            >
                <!-- <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
                ></v-img> -->

            <v-card-title
            class="cardText">
            Synergy
            </v-card-title>

            <v-card-subtitle
            class="cardText">
            Project Management App
            </v-card-subtitle>

            <v-card-actions>
            <v-btn
                color="orange lighten-2"
                text
                @click="navigateSynergyFe()"
                class="gitLink"
            >
                Link to FE GitHub
            </v-btn>
            <v-btn
                color="orange lighten-2"
                text
                @click="navigateSynergyBe()"
                class="gitLink"
            >
                Link to BE GitHub
            </v-btn>

            <v-spacer></v-spacer>

            <v-btn
                icon
                @click="show3 = !show3"
            >
            <v-icon>{{ show3 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
            </v-btn>
            </v-card-actions>

            <v-expand-transition>
            <div v-show="show3">
            <v-divider></v-divider>

            <v-card-text
            class="cardText">
            For my MVP project, I built a project Management application. There are 3 authentication levels for users, Organization Owners, Project Managers and Employees. Each our able to do operate the differing CRUD operations based on their token credentials. Owners and Project Managers can create Projects and tasks for their teams and communicate through comments in the tasks. 
            <p>Skills:  HTML, CSS, SCSS, JavaScript, Vue.js, Python, Flask, Pinia, MariaDB, SQL, APACHE </p>
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>
        </v-container>
    </v-container>
</template>

<script>
    export default {
        name: "MyProjects",
        data: () => ({
        show1: false,
        show2: false,
        show3: false
        }),
        methods: {
            navigateSynergyFe() {
                window.open('https://github.com/ericstretton/synergy_frontend')
            },
            navigateSynergyBe() {
                window.open('https://github.com/ericstretton/mvp_project_BE')
            },
            navigateFoodieFe() {
                window.open('https://github.com/ericstretton/foodie-project')
            },
            navigateFoodieBe() {
                window.open('https://github.com/ericstretton/backend_foodie')
            },
            navigatePizzaRicks(){
                window.open('https://github.com/ericstretton/PizzaProject')
            }
        }
    }
</script>

<style lang="scss" scoped>
#projectContainer{
    display: grid;
    grid-template-columns: 0.5fr 1fr 1fr 1fr 0.5fr;

    .gitLink{
        font-size: 0.75em;
    }
    .cardText{
        color: whitesmoke;
        opacity: 0.75;
    }
    .cards{
        background-color:#343030;
        border: 2px solid whitesmoke;
    }
    #foodie{
        grid-column: 3;
    }
    #pizzaRicks{
        grid-column: 2;
    }
    #synergy{
        grid-column: 4;
    }
}
.font_color{
    color: #6aaaff;
}
</style>