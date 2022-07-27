<template>
    <v-container>
        <v-subheader class="text-center justify-center py-6">
            <h3 class="font-weight-bold text-h3 font_color">
                About Me
            </h3>
        </v-subheader>
        <v-container id="meContainer">
            <div id="mePhoto">
                <img src="https://media-exp1.licdn.com/dms/image/C5603AQFSi5r0KY0caw/profile-displayphoto-shrink_200_200/0/1653407415608?e=1664409600&v=beta&t=i46xsaUzcyKXz_PbKxWBa8yL6x9CmmIMgLESSPgR_2Y" alt="EricPhoto">
            </div>
            <div id="meText">
                <p> I'm Eric Stretton, a Full stack Web Developer based in Saskatoon, SK. I graduated from Innotech College with a diploma in Full-Stack Development in July 2022. </p>
                <p> I was drawn to the tech industry through past work as a data entry clerk, as such, I am very driven towards backend development. Nonetheless, I enjoy programming regardless of what side of the tech stack I am able to work with as any opportunity to code is another chance at learning something new! </p>
                <p> I am dedicated to being a lifelong learner. 
                    When I am not coding, I enjoy playing with my cats Ted and Maeve. I also enjoy long walks where I can take a step back and reflect on the problems I am solving. </p>
            </div>
        </v-container>
    </v-container>
</template>

<script>
    export default {
        name: "AboutMe"
    }
</script>

<style lang="scss" scoped>
.font_color{
    color: #6aaaff;
}
#meContainer{
    display: grid;
    grid-template-columns: 0.5fr 1fr 1fr 0.5fr;
    column-gap: 5px;
    #mePhoto{
        border: 2px solid whitesmoke;
        border-radius: 5px;
        grid-column: 2;
        background-color: #343030;
        justify-self: center;
        align-self: center;
        
    }
    #meText{
        border: 2px solid whitesmoke;
        border-radius: 5px;
        grid-column-start: 3;
        grid-column-end: 5;
        background-color: #343030;
        p{
            color: whitesmoke;
            opacity: 0.75;
        }
    }
}
</style>