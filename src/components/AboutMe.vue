<template>
    <v-container>
        <v-subheader class="text-center justify-center py-6">
            <h3 class="font-weight-bold text-h3 font_color">
                About Me
            </h3>
        </v-subheader>
        <v-container id="meContainer">
            <div id="mePhoto">
                <img src="" alt="EricPhoto">
            </div>
            <div id="meText">
                <p>Content About Eric and such</p>
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
    }
    #meText{
        border: 2px solid whitesmoke;
        border-radius: 5px;
        grid-column: 3;
    }
}
</style>