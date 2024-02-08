<template>
  <main class="main-container">
    <section class="content-container">
      <section class="container">
        <div id="about">
          <h1>About</h1>
          <p>Hello!</p>
          <p>I'm Geoff Kevin G. Apologista, a fourth-year Computer Science student from the University of San Agustin Inc. With a strong passion for coding and a desire to become a well-rounded developer, I am actively working towards becoming a full-stack professional. In my portfolio, I showcase my projects and skills in various programming languages and technologies, demonstrating my commitment to creating innovative solutions across different domains, including web development, game development, and software engineering.</p>
          <p>When I'm not coding, I cook, play video games and basketball.</p>
          <p>Being someone who is committed to continuous learning, I am constantly in pursuit of fresh knowledge and experiences that can expand my outlook and improve my abilities.</p>
          <p>I appreciate your effort in getting to know me better!</p>
        </div>
        </section>
        <section class="container">
          <div id="skills">
            <h1>Skills</h1>
            <div>
              <progressBar :progressData="progressData"></progressBar>
            </div>
          </div>
        </section>
        <section class="container">
          <div id="projects">
            <h1>Projects</h1>
          </div>
        </section>
        <section class="container">
          <div id="education">
            <h1>Education</h1>
          </div>
        </section>
    </section>
  </main>
  <SidebarComponent />
</template>

<script>
import ProgressBar from './components/ProgressBars.vue'
import SidebarComponent from './components/SidebarComponent.vue'

export default {
  name: 'HomeView',
  components: {
    ProgressBar,
    SidebarComponent
  },
  data () {
    return {
      progressData: [
        { title: 'HTML - CSS - JavaScript', progress: 70, color: '#2c98f0' },
        { title: 'Vue.js', progress: 45, color: '#ec5453' },
        { title: 'Node.js', progress: 45, color: '#f9bf3f' },
        { title: 'Laravel', progress: 30, color: '#f9bf3f' },
        { title: 'MongoDB', progress: 30, color: '#2fa499' },
        { title: 'GitHub', progress: 70, color: '#a84cb8' },
        { title: 'VSCode', progress: 80, color: '#a84cb8' }
      ]
    }
  }
}
</script>

<style lang="scss">

  #app {
    background-color: #12372A;
  }

  .main-container {
    margin-top: -10px;
    margin-bottom: -10px;
    display: flex;
  }

  .container {
    padding: 0 2.0em;
    margin-bottom: 40px;
  }

  .content-container {
    flex-grow: 1;
    margin-top: 32px;
    margin-left: 300px;
  }

  h1 {
    font-family: 'Montserrat', sans-serif, monospace;
    font-size: 36px;
    text-align: left;
    color: #FBFADA;
    margin: 0 0 24px 0;
  }

  p {
    font-family: 'Montserrat', sans-serif, monospace;
    font-size: 16px;
    line-height: 1.5;
    text-align: left;
    color: #FBFADA;
    margin: 0 0 16px 0;
  }

</style>
