<template>
  <div id="app">
    <!-- Navbar -->
    <nav class="navbar navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Portofolio</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Burger menu: muncul di semua ukuran layar -->
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" href="#skills">Skills</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#certificates">Sertifikat</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#experience">Pengalaman Kerja</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#projects">Proyek</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Kontak</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Content -->
    <div class="container mt-4">
      <h1>Mufti Purwalaksana</h1>
      <p>
        Saya seorang IT Support & Web Developer yang pernah bekerja di
        <a href="https://remula-inti.com/" target="_blank">PT Remula</a>.
      </p>

      <!-- Skills -->
      <section id="skills">
        <h2>Skills</h2>
        <ul>
          <li>HTML, CSS, JavaScript</li>
          <li>React, Laravel, PHP</li>
          <li>MySQL, Git, GitHub, WordPress</li>
          <li>REST API, Bootstrap</li>
        </ul>
      </section>

      <!-- Certificates -->
      <section id="certificates">
        <h2>Sertifikat</h2>
        <div v-for="(certificate, index) in certificates" :key="index" class="mb-2">
          <button
            class="btn btn-primary"
            @click="openLink(certificate.url)"
          >
            {{ certificate.title }}
          </button>
        </div>
      </section>

      <!-- Experience -->
      <section id="experience">
        <h2>Pengalaman Kerja</h2>
        <ul>
          <li><strong>IT Support – PT Remula</strong> (2016 – 2021)</li>
          <li><strong>Web Developer – PT Remula</strong> (2021 – 2024)</li>
        </ul>
      </section>

      <!-- Projects -->
      <section id="projects">
        <h2>Proyek</h2>
        <div v-for="(project, index) in projects" :key="index" class="mb-2">
          <button
            class="btn btn-primary"
            @click="openLink(project.url)"
          >
            {{ project.title }}
          </button>
        </div>
      </section>

      <!-- Contact -->
      <section id="contact">
        <h2>Kontak</h2>
        <button
          class="btn btn-primary"
          @click="openLink('mailto:muftipurwalaksana5@gmail.com')"
        >
          Kirim Email
        </button>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      certificates: [
        {
          title: 'Responsive Web Design – freeCodeCamp',
          url: 'https://www.freecodecamp.org/certification/fccfc107e90-7772-49db-a0db-04f5eb78935a/responsive-web-design',
        },
        {
          title: 'JavaScript Algorithms and Data Structures – freeCodeCamp',
          url: 'https://www.freecodecamp.org/certification/your-username/javascript-algorithms',
        },
        {
          title: 'Front End Libraries – freeCodeCamp',
          url: 'https://www.freecodecamp.org/certification/your-username/front-end-libraries',
        }
      ],
      projects: [
        {
          title: 'Remula Gudang – Aplikasi Pergudangan',
          url: 'https://github.com/muftip/Remula-gudang',
        },
        {
          title: 'Absensi – Laravel + Breeze',
          url: 'https://github.com/muftip/absensi',
        },
     
      ]
    };
  },
  methods: {
    openLink(url) {
      window.open(url, '_blank');
    }
  }
};
</script>

<style scoped>
/* Style opsional */
</style>
