<template>
    <div class="container-fluid" style="margin-top: 70px;">
    <div id="all-projects">

        <div class="project">
            <div class="pro-img">
                <img src="../assets/images/projects/3columns.jpg" alt="description">
            </div>
            <div class="pro-data">
                <div class="pro-links">
                    <div class="ref-1">
                    <button id="proButton"><a id="siteLink" href="https://kareemiswebdevelper.github.io/threeColumnsPage/">Preview Site</a></button>
                    </div>
                    <div class="ref-2">
                        <a href="https://github.com/kareemIsWebDevelper/threeColumnsPage"><i class="bi bi-github"></i></a>
                    </div>
                </div>
            </div>
        </div>
        <div class="project">
            <div class="pro-img">
                <img src="../assets/images/projects/desktop-active-state.jpg" alt="description">
            </div>
            <div class="pro-data">
                <div class="pro-links">
                    <div class="ref-1">
                    <button id="proButton"><a id="siteLink" href="https://kareemiswebdevelper.github.io/thought-to-select-furniture/">Preview Site</a></button>
                    </div>
                    <div class="ref-2">
                        <a href="https://github.com/kareemIsWebDevelper/thought-to-select-furniture"><i class="bi bi-github"></i></a>
                    </div>
                </div>
            </div>
        </div>
        <div class="project">
            <div class="pro-img">
                <img src="../assets/images/projects/desktop-design.jpg" alt="description">
            </div>
            <div class="pro-data">
                <div class="pro-links">
                    <div class="ref-1">
                        <button id="proButton"><a id="siteLink" href="https://kareemiswebdevelper.github.io/comming-apparel/">Preview Site</a></button>
                    </div>
                    <div class="ref-2">
                        <a href="https://github.com/kareemIsWebDevelper/comming-apparel"><i class="bi bi-github"></i></a>
                    </div>
                </div>
            </div>
        </div>
        
    </div> 
    </div>
</template>


<style>
    .pro-header h1 {
    text-align: center;
    margin-bottom: 50px;
}

#all-projects {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 40px;
}

.project {
    width: 400px;
    height: 400px;
    display: flex;
    flex-flow: column;
    border-radius: 20px;
    border: 1px solid darkgrey;
}
.pro-img {
    width: 400px;
    height: 300px;
    border-radius: 20px;
    margin-bottom: 50px;
}

.pro-img img {
    background-size: 100% 100%;
    width: 400px;
    height: 300px;
    border-radius: 20px 20px 0 0;
}

.pro-data {
    width: inherit;
    min-height: 130px;
    background-color: white;
    border-radius: 0 0 20px 20px;
}

.pro-details {
    text-align: center;
}

.pro-links {
    display: flex;
    justify-content: space-around;
    align-items: center;
}


#proButton {
    border-radius: 10px;    
    border: none;
    width: 130px;
    height: 40px;
    background-color: darkcyan;
}

#proButton:hover {
    cursor: pointer;
    opacity: .5;
}

.ref-2 i {
    font-size: 40px;
    color: black;
}


#siteLink {
    text-decoration: none;
    color: white;
    font-weight: bold;
}



@media screen and (max-width: 400px) {
    #all-projects {
        gap: 70px;
        margin: auto;
        display: grid;
        place-items: center;
    }

    .pro-header h1 {
        text-align: center;
        margin-bottom: 50px;
    }
    
    .project,
    .pro-img,
    img,
    .pro-data{
        max-width: 350px;
    }

    /* .pro-img img {
        width: 300px;
        background-size: 100% 100%;
    }

    .pro-data {
        max-width: 300px;
    } */
}
</style>