<template>
    <div class="beetwen">
        <div class="leftM">
            <h1>{{ nama }}</h1>
            <h4>{{ job }}</h4>
            <button class="huba">Contact Me</button>
        </div>
        <div class="rightM">
            <img src="/gambar/fadel1.png" alt="" class="gambarF">
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            nama: 'Fadel Muhammad',
            job: 'Junior Programmer',
            aboutMe: ''
        }
    },
}
</script>

<style scoped>
.beetwen {
    display: flex;
    margin: 100px 0;
}

.leftM {
    width: 100%;
    padding: 70px 0;

}

.leftM h1 {
    font-size: 50px;
    font-weight: bold;
}

.leftM h4 {
    font-size: 30px;
}

.rightM {
    width: 100%;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 0 0 100px;
}

.huba {
    width: 150px;
    font-weight: bolder;
    color: white;
    padding: 10px 0;
    margin: 80px 0;
    background-color: green;
    border-radius: 30px;
}

.gambarF {
    width: 350px;
    height: 400px;
    background-color: gray;
    border-radius: 100px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(5, 206, 65, 0.4);
}

@media (max-width: 768px) {
    .beetwen {
        flex-direction: column;
        /* Stack elements vertically */
        text-align: center;
        /* Center text for better mobile view */
        margin: 0;
    }

    .rightM {
        padding: 0;
        /* Remove padding on mobile */
    }

    .gambarF {
        align-items: center;
        /* Add some space above the image */
    }
}

@media (max-width: 400px) {
    .beetwen {
        flex-direction: column;
        text-align: center;
        margin: 0;
    }

    .leftM h1 {
        font-size: 30px;
        font-weight: bold;
    }

    .leftM h4 {
        font-size: 20px;
    }

    .rightM {
        padding: 0;
        /* Remove padding on mobile */
    }

    .gambarF {
        align-items: center;
        width: 300px;
        height: 350px;
        border-radius: 70px;
        /* Add some space above the image */
    }
}
</style>