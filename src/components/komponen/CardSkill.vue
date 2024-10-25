<template>
    <div class="container">
        <div class="card" v-for="(item, card) in cards" :key="card">
            <img :src="item.image" alt="" class="card-image">
            <h2>{{ item.title }}</h2>
        </div>
    </div>
</template>

<script>
export default {
    props: ['cards'],
    data() {
        return {
            
        }
    },
}
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap; /* Allow cards to wrap */
}

.card {
  width: 250px;
  height: 200px; /* Adjust height as needed */
  background: linear-gradient(135deg, rgba(255, 255, 255, 0.5), rgba(1, 19, 4, 0.5));
  margin: 0 30px 30px; /* Add margin to bottom for spacing */
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  overflow: hidden;
  transition: box-shadow 0.3s ease-in-out;
  position: relative; /* Added for pseudo-element */
}

.card-image {
    width: 100px;
    height: auto;
    border-radius: 10px;
    margin: 10px 0 0 0;
    /* Space between image and text */
}

.card:before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: 10px;
    /* background: linear-gradient(45deg, rgba(255, 255, 255, 0) 0%, rgba(255, 105, 180, 0.5) 100%); */
    filter: blur(10px);
    z-index: -1;
    opacity: 0.7;
}

.card:hover {
    box-shadow: 0 0 50px rgba(14, 107, 14, 0.5);
}

@media (max-width: 768px) {
    .container {
        align-items: center;
    }
    .card {
        width: 150px;
        height: 100px;
    }
    .card-image {
        width: 25px;
        height: 25px;
    }
    h2 {
        font-size: 12px;
        /* display: none; */
    }
}

@media (max-width: 400px)
{
    .container {
        align-items: center;
    }
    .card {
        width: 100px;
        height: 100px;
    }
    .card-image {
        width: 25px;
        height: 25px;
        margin: 0;
    }
    h2 {
        font-size: 10px;
        /* display: none; */
    }
}
</style>