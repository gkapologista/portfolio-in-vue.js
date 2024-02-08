<template>
  <div class="sidebar">
    <div class="logo-container">
      <img alt="profile-img" class="logo" src="../assets/images/logo.webp">
    </div>
    <h3>Geoff Kevin G. Apologista</h3>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#education">Education</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'SidebarComponent'
}
</script>

<style lang="scss">
.logo {
  border-radius: 25px;
  height: 250px;
}

.logo-container {
  display: flex;
  justify-content: center;
  margin: 32px 0 20px 0;
}

.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 300px;
  height: 100%;
  background-color: #436850;
  color: #fff;
  overflow-y: auto;
}

.sidebar h3 {
  font-family: 'Montserrat', sans-serif, monospace;
  margin: 0;
  padding: 20px;
  font-size: 32px;
  color: #FBFADA;
  text-align: center;
}

.sidebar ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.sidebar li {
  padding: 10px;
  font-size: 18px;
  text-align: center;
}

.sidebar a {
  font-family: 'Montserrat', sans-serif, monospace;
  font-size: 16px;
  color: #FBFADA;
  text-decoration: none;
}

.sidebar a:hover {
  color: #f9bf3f;
  transition: all 0.3s ease;
}

</style>
