<template>
  <div id="app">
    <!-- Navbar -->
    <nav class="navbar navbar-light bg-dark shadow-sm border-bottom border-2 border-secondary">
      <div class="container-fluid">
        <a class="navbar-brand fs-3 fw-bold text-white" href="#">Portofolio</a>
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

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link text-white" href="#skills">Skills</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="#certificates">Sertifikat</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="#experience">Pengalaman Kerja</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="#projects">Proyek</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="#contact">Kontak</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Content -->
    <div class="container py-5">
      <h1 class="display-4 text-center mb-4">Mufti Purwalaksana</h1>
      <p class="lead text-center mb-5">
  Saya adalah seorang IT Support dan Web Developer dengan pengalaman di dalam perusahaan bergerak di bidang manufaktur pembuatan alat pabrikasi. 
  Selama karir saya, saya telah berkontribusi di <a href="https://remula-inti.com/" target="_blank">PT Remula</a>, 
  tempat saya mengembangkan dan mengelola aplikasi berbasis web, memberikan dukungan teknis, serta berperan dalam pemeliharaan sistem dan infrastruktur teknologi informasi.
</p>


      <!-- Skills -->
      <section id="skills" class="my-5 py-5 px-4 border border-secondary rounded">
        <h2>Skills</h2>
        <ul>
          <li>HTML, CSS, JavaScript</li>
          <li>React, Laravel, PHP</li>
          <li>MySQL, Git, GitHub, WordPress</li>
          <li>REST API, Bootstrap, React.js</li>
        </ul>
      </section>

      <!-- Certificates -->
      <section id="certificates" class="my-5 py-5 px-4 border border-secondary rounded">
        <h2>Sertifikat</h2>
        <div class="d-grid gap-3">
          <!-- Sertifikat lama (Responsive Web Design) -->
          <button class="btn btn-primary" onclick="window.open('https://www.freecodecamp.org/certification/fccfc107e90-7772-49db-a0db-04f5eb78935a/responsive-web-design')">
            Responsive Web Design – freeCodeCamp
          </button>
          <!-- Sertifikat baru 1 (Git) -->
          <button class="btn btn-primary" onclick="window.open('https://www.dicoding.com/certificates/81P2OD4Y4XOY')">
            Belajar Dasar Git dengan GitHub – Dicoding
          </button>
          <!-- Sertifikat CodePolitan -->
          <button class="btn btn-primary" onclick="window.open('https://www.codepolitan.com/coders/Mufti16/')">
            CodePolitan – Profil Sertifikat
          </button>
        </div>
      </section>

      <!-- Experience -->
      <section id="experience" class="my-5 py-5 px-4 border border-secondary rounded">
        <h2>Pengalaman Kerja</h2>
        <ul>
          <li><strong>IT Support – PT Remula</strong> (2016 – 2021)</li>
          <li><strong>Web Developer – PT Remula</strong> (2021 – 2024)</li>
        </ul>
      </section>

      <!-- Projects -->
      <section id="projects" class="my-5 py-5 px-4 border border-secondary rounded">
        <h2>Proyek</h2>
        <div class="d-grid gap-3">
          <button class="btn btn-primary" onclick="window.open('https://github.com/muftip/Remula-gudang')">
            Remula Gudang – Aplikasi Pergudangan
          </button>
          <button class="btn btn-primary" onclick="window.open('https://github.com/muftip/absensi')">
            Absensi – Aplikasi Presensi Laravel + Vue
          </button>
          <button class="btn btn-primary" onclick="window.open('https://github.com/muftip/buku-tamu')">
            Buku Tamu – Laravel Breeze dan Vue
          </button>
        </div>
      </section>

      <!-- Contact -->
      <section id="contact" class="my-5 py-5 px-4 border border-secondary rounded">
        <h2>Kontak</h2>
        <div class="d-flex flex-column gap-3">
          <button class="btn btn-primary" onclick="window.location.href='mailto:muftipurwalaksana5@gmail.com'">
            Kirim Email
          </button>
          <button class="btn btn-info text-white" onclick="window.open('https://www.linkedin.com/in/mufti-purwalaksana-26990a162/')">
            LinkedIn – Mufti Purwalaksana
          </button>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style scoped>
body {
  font-size: 16px;
}

@media (max-width: 576px) {
  body {
    font-size: 17px;
  }
  h1, h2 {
    font-size: 1.75rem;
  }
  .navbar-brand {
    font-size: 1.5rem !important;
  }
  .btn {
    font-size: 1rem;
  }
}

@media (min-width: 577px) {
  h1, h2 {
    font-size: 2rem;
  }
  .btn {
    font-size: 1.1rem;
  }
}

.navbar-toggler {
  border-color: white;
}

.navbar-toggler-icon {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 30 30' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba%28255, 255, 255, 1%29' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3E%3C/svg%3E");
}
</style>
