<template>
    <header>
        <img src="@/assets/header-image3.png" alt="Header" />

        <v-container fluid>
            <v-row justify="center">
                <v-col cols="12" class="text-xs-center" sm="8" md="6" lg="4" xl="3" offset-sm="2" offset-md="3"
                    offset-lg="4" offset-xl="4">
                    <v-card class="resizable-box" :style="{ backgroundImage: 'url(' + backgroundImage + ')' }">
                        <v-card-title class="text-container">Lilla Ajándékbolt
                            <br>Lillafüred<br><br></v-card-title>
                        <v-card-title class="text-container2">3517 Miskolc, Pávai Vajna Ferenc sétány<br>

                            Nyitvatartás:<br>

                            H-V: 9:45 - 16:30<br>

                            Tel. 0036/30-426-6078</v-card-title>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>

    </header>
</template>

<script>
export default {
    data() {
        return {
            backgroundImage: require('@/assets/title2.png'),
        };
    },
};
</script>
  
<style scoped>
header {
    width: 100%;
    height: auto;
    min-height: 684px;
    overflow: hidden;
}

img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

@media (max-width: 768px) {
    img {
        height: auto;
    }
}



.resizable-box {
    overflow: hidden;
    transition: width 0.3s ease, height 0.3s ease;
    position: absolute;
    top: 30%;
    left: 24%;
    transform: translate(-50%, -50%);
    text-align: center;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 2em;
    padding-left: 4em;
    padding-right: 4em;
}

.text-container {
    font-family: 'Futura', sans-serif;
    text-align: center;
    letter-spacing: 0.1em;
    /* Character spacing */
    font-weight: 400;
    font-size: 2.6em;
    /* Initial font size */
    transition: font-size 0.3s ease;
    color: #7F703D;
    /* Smooth transition effect */
}
.text-container2 {
    font-family: 'Futura', sans-serif;
    text-align: center;
    /* Character spacing */
    font-weight: 500;
    font-size: 1em;
    /* Initial font size */
    transition: font-size 0.3s ease;
    color: #7F703D;
    /* Smooth transition effect */
}
</style>
  