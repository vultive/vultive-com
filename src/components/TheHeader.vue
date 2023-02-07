<template>
  <header class="sticky-top">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img
            src="/static/logos/vultive.png"
            width="156"
            height="40"
            class="d-block"
            alt="Vultive Logo"
            loading="lazy"
          />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#services">Services</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="https://vultive.betteruptime.com"
                >Status</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
  <div class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner vultive-carousel">
      <div class="carousel-item active">
        <img
          :src="require('@/assets/header.jpg')"
          class="d-block w-100 h-100 vultive-obj-cover"
          alt="Header"
        />
      </div>
    </div>
  </div>
  <section class="bg-dark text-light">
    <div class="container py-4">
      <div class="row align-items-center text-center">
        <div class="col-md-6">
          <p class="fs-4 d-inline">Many services, one account.</p>
        </div>
        <div class="col-md-6">
          <a
            href="https://my.vultive.com/register"
            class="btn btn-lg btn-outline-light mt-2 m-md-0"
            >Join now</a
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Components - TheHeader",
};
</script>
