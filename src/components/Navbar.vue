<template>
    <div>
    <nav class="navbar navbar-expand-lg bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Logo - CCBA</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page"><RouterLink to="/">Tela de Login</RouterLink></a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" aria-current="page"><RouterLink to="/ListView">Listar</RouterLink></a>
        </li>
        <li class="nav-item">
          <a class="nav-link active" aria-current="page"><RouterLink to="#">Outro</RouterLink></a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Pesquisar" aria-label="Pesquisar">
        <button class="btn btn-outline-success" type="submit">Pesquisar</button>
      </form>
    </div>
  </div>
</nav>
        
    </div>
</template>

<script>

</script>

<style>


</style>