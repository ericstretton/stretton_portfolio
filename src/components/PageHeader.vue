<template>
        
        <v-app-banner 
        class="banner"
        >
            <v-parallax
            dark
            height="25%"
            src="https://img.freepik.com/free-vector/hazy-black-ink-texture-with-brushstrokes_125540-1360.jpg?w=1380&t=st=1658873055~exp=1658873655~hmac=8b894974cb761bd9dbc3ed7951fe249b08e647b88cce44deb071a3fb3fb9161f">
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