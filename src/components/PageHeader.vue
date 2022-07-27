<template>
        
        <v-app-banner 
        class="banner"
        >
            <v-parallax
            dark
            height="25%"
            src="https://cdn.wallpapersafari.com/37/9/Yj3WSM.jpg">
            <v-app-bar-title class="text-center justify-center ">
                <h1 class="font-weight-bold text-h2 font_color">
                Eric Stretton
                </h1>
            </v-app-bar-title>

            <v-subheader class="text-center justify-center py-6">
                <h3 class="font-weight-bold text-h6 font_color">
                    Full-Stack Developer
                </h3>
            </v-subheader>

            <v-tabs
            v-model="tab"
            background-color="transparent"
            color="#6aaaff"
            theme="white"
            grow
            >
            <v-tab
                v-for="item in items"
                :key="item"
                class="font_color"
            >
                {{ item }}
            </v-tab>
            </v-tabs>

            <v-tabs-items v-model="tab">
            <v-tab-item
                v-for="item in items"
                :key="item"
                color="#6aaaff"
            >
                
            </v-tab-item>
            </v-tabs-items>
            </v-parallax>
        </v-app-banner>
        
    
</template>

<script>
    export default {
        name: "PageHeader",
        data () {
            return {
                tab: null,
                items: [
                    'Top', 'About Me', 'Projects', 'Contact',
                ],
                }
        },
    }
</script>

<style lang="scss" scoped>

.font_color {
  color: #6aaaff !important;
}
.banner{
    max-width: 100%;
    
}
</style>