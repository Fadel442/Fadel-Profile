<template>
    <div class="between">
        <div class="leftM">
            <img src="/gambar/fadel.png" alt="" class="gambarF">
        </div>
        <div class="RightM">
            <div class="titles">
                <h1>About Me</h1>
                <p>I'm a passionate software engineer and game developer with a keen interest in augmented reality,
                    virtual reality, and web development. I recently graduated from Telkom University, Surabaya Campus,
                    with a degree in Software Engineering, and over the past year, I've gained valuable experience in
                    creating engaging, interactive learning experiences through AR/VR and game development. Alongside
                    these interests, I enjoy working with frameworks like Vue.js, Laravel, and Vite, blending creativity
                    with structured code to build responsive, user-friendly applications. My skillset also includes
                    proficiency in HTML, CSS, PHP, and JavaScript, which form the backbone of my web development
                    toolkit. Driven by curiosity and a dedication to both web and game development, I’m constantly
                    exploring new technologies to create impactful digital experiences.</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.titles {
    margin: 50px 0;
    text-align: justify;
}

.titles h1 {
    font-size: 30px;
}

.titles p {
    font-size: 20px;
}

.between {
    display: flex;
    margin: 100px 0;
}

.leftM {
    width: 20%;
    justify-content: left;
    align-items: center;
    text-align: center;
    padding: 0 500px 0 0;
}

.rightM {
    width: 100%;
    padding: 0 100px;
}

.gambarF {
    width: 350px;
    height: 500px;
    background-color: gray;
    border-radius: 100px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(5, 206, 65, 0.4);
}

@media (max-width: 768px) {
    .between {
        flex-direction: column;
        align-items: center;
        margin: 0;
    }

    .titles {
        margin: 50px 20px;
        text-align: center;
    }
    .titles h1 {
        font-size: 25px;
    }
    .titles p {
        font-size: 15px;
    }

    .leftM {
        width: 100%;
        /* Full width on mobile */
        padding: 0;
        /* Remove padding */
    }

    .rightM {
        width: 100%;
        /* Full width on mobile */
        padding: 0;
        /* Remove padding */
        text-align: center;
        /* Center text on mobile */
    }

    .gambarF {
        display: none;
    }
}

@media (max-width: 400px) {
    .between {
        flex-direction: column;
        align-items: center;
        margin: 0;
    }

    .titles h1 {
        font-size: 20px;
    }

    .titles p {
        font-size: 10px;
    }
}
</style>