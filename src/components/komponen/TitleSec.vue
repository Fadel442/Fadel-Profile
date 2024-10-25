<template>
    <div class="skill-sec">
      <div class="blok1">
        
      </div>
      <div>
        <h1>{{ skill }}</h1>
      </div>
      <div class="blok2">

      </div>
    </div>
</template>

<script>
export default{
    props: ['skill']
}
</script>

<style scoped>
.skill-sec {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;
}
.blok1, .blok2{
  height: 5px;
  width: 100%;
  margin: 0 50px;
  border-radius: 100px;
  background-color: gray;
}
h1 {
    text-align: center; 
    font-size: 20px; 
    font-weight: bold;
}
</style>