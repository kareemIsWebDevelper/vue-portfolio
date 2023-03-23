<script>
    import myImage from './myImage.vue'

    export default {
        components: {
            myImage,
        }
    }
</script>

<template>
    <div class="container">
        <div class="frame">
            <myImage />
        </div>            
        <div id="card" class="card text-center p-3">
            
            <div>
                <h1>Fullstack Developer</h1>
                <p>I'm developing websites using Nuxt.js</p>
                <p class="mr-4" style="margin-top: -15px;">framework with at the client side,</p>
                <p style="margin-top: -15px;">Django framework at the server side.</p>
            </div>
            <RouterLink to="/about" role="button">About Me</RouterLink>

            <div class="flex">
                <div>
                    <p>4 years</p>
                    <p class="assesment">Experience</p>
                </div>
                <div>
                    <p>50+</p> 
                    <p class="assesment">Projects</p>
                </div>
                <div>
                    <p>99%</p>
                    <p class="assesment">Satisfaction</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

.container {
   display: flex;
   justify-content: space-around;
   align-content: flex-end;
   margin-right: 170px;
}
.about {
   display: grid;
   place-items: center;
   align-items: space-between;
}

.flex {
    display: flex;
    gap: 20px;
    justify-content: flex-start;
    align-items: flex-start;
    margin-bottom: -20px;
}


a {
    color: white;
    background-color: darkcyan;
    width: 100px;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: -20px 0 0 0;
}
.assesment {
    margin-top: -20px;
}

@media screen and (max-width: 400px) {
    .container {
        display: grid;
        border-radius: 20px;
    }

    #header h1 {
        font-weight: bold;
        font-size: 30px;
        margin-bottom: -20px;
    }

    #header br {
        display: block;
    }

    .right div:nth-child(1),
    div:nth-child(3){
        margin: auto;
    }

    a { 
        margin: 20px auto 20px auto;
        width: 280px;
    }
}

@media screen and (min-width: 1000px) {
    #card {
        width: 500px;
        display: grid;
        place-items: center;
        margin-top: 30px;
    }
}
</style>