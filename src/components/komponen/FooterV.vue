<template>
  <footer class="footer">
    <div class="footer-content">
      <p>&copy; 2024 J-Smaruna. All rights reserved.</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 20px 0;
  position: relative;
  bottom: 0;
  width: 100%;
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}


.footer-links a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .footer-content {
    font-size: 15px;
  }
}

@media (max-width: 400px) {
  .footer-content {
    font-size: 10px;
  }
}
</style>