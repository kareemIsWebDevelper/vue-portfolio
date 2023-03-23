<template>
    <div id="skills" class="card text-center bg-white mt-3">
        <div class="card-body">
            <div>
                <h3 class="card-header mb-3">Client Side</h3>
                <div id="skills" class="flex">
                    <img src="../assets/images/nuxt.jpeg">
                    <img src="../assets/images/vue.jpeg">
                    <img src="../assets/images/ts.jpeg">
                    <img src="../assets/images/js.jpeg">
                    <img src="../assets/images/css.jpeg">
                    <img src="../assets/images/html.jpeg">
                </div>
            </div>
            <div>
                <h3 class="card-header mt-3">Server Side</h3>
                <div id="skills" class="flex">
                    <img src="../assets/images/django.jpeg">
                    <img src="../assets/images/python.jpeg">
                </div>
            </div>
        </div>
    </div>
</template>

<scipts>

</scipts>

<style scoped>
    #skills {
        display: grid;
        place-items: center;
        justify-items: center;
    }
    .flex {
        display: flex;
        flex-wrap: wrap;
        gap: 15px;
    }

</style>