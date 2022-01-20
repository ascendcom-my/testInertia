<template>
  <main class="flex flex-col h-screen">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <inertia-link href="/" class="nav-item nav-link">Home</inertia-link>
          <inertia-link href="/users"  class="nav-item nav-link">Index</inertia-link>
        </div>
      </div>
    </nav>

    <article class="flex-1">
      <slot />
    </article>
  </main>
</template>

<script>
    export default {
    }

</script>

