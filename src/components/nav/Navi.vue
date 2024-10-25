<template>
    <nav>
    <div class="container">
        <div>
            <h1>FD</h1>
        </div>
        <div class="cont1">
            <RouterLink to="/">
                <img src="/icon/ic_linkedin.png" alt="">
            </RouterLink>
            <RouterLink to="/">
                <img src="/icon/ic_github.png" alt="">
            </RouterLink>
            <RouterLink to="/">
                <img src="/icon/ic_instagram.png" alt="">
            </RouterLink>
        </div>
    </div>
    </nav>
</template>

<style>
.container{
  display: flex;
  padding: 20px 0;
  justify-content: space-between;
  align-items: center;
  text-align: center;
  color: white;
}
h1 {
  font-size: 25px;
  font-weight: bold;
}
nav {
  width: 100%;
  font-size: 20px;
  margin-bottom: 50px;
}

nav a {
  display: inline-block;
  padding: 0 10px;
}
img {
  width: 30px;
  height: 30px;
}

/* Responsive styles */
@media (max-width: 768px) {
  .container {
    flex-direction: row; /* Stack items vertically on mobile */
    padding: 20px 100px;
    align-items: center; /* Center items */
  }

  nav {
    margin-bottom: 20px;
  }
}
</style>