<template>
    <div class="between">
        <div class="leftM">
            <div class="titles">
                <h1>J-Smaruna</h1>
                <p>J-Smaruna is an innovative Android app designed to make learning Japanese characters—Hiragana,
                    Katakana, and basic Kanji—both engaging and interactive. By harnessing augmented reality with
                    Vuforia, J-Smaruna brings Japanese characters to life, allowing users to explore and memorize them
                    visually in an immersive way. This app supports students in developing their Japanese language
                    skills by combining technology and education in a user-friendly experience.</p>
                <button>Click Here!</button>
            </div>
        </div>
        <div class="RightM">
            <img src="/gambar/jsmaruna.png" alt="" class="gambarF">
        </div>
    </div>
</template>

<style scoped>
.titles {
    margin: 30px 0;
    text-align: justify;
}

.titles h1 {
    font-size: 30px;
}

.titles p {
    font-size: 20px;
}

.titles button {
    width: 150px;
    font-weight: bolder;
    color: white;
    padding: 10px 0;
    margin: 80px 0;
    background-color: green;
    border-radius: 30px;
}

.between {
    display: flex;
    margin: 100px 0;
}

.leftM {
    width: 100%;
    padding: 100px 100px 0 0;
}

.rightM {
    width: 20%;
    justify-content: left;
    align-items: center;
    text-align: center;
    /* padding: 0 0 0 100px; */

}

.gambarF {
    width: 350px;
    height: 500px;
    filter: drop-shadow(10px 5px 10px rgba(55, 224, 13, 0.3));
}

@media (max-width: 1080px) {
    .between {
        flex-direction: column;
        align-items: center;
        margin: 0 0;
    }

    .titles h1 {
        font-size: 25px;
    }

    .titles p {
        font-size: 15px;
    }

    .leftM {
        padding: 0;
    }

    .titles {
        text-align: center;
    }

    .gambarF {
        width: 300px;
        height: 450px;
        border-radius: 60px;
        margin-bottom: 50px;
    }
}

@media (max-width: 400px) {
    .titles h1 {
        font-size: 20px;
    }

    .titles p {
        font-size: 10px;
    }
    .gambarF {
        display: none;
    }
}
</style>