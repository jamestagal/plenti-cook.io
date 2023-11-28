<script>
  let activeItem = { id: "home", isActive: true };

  function setActive(item) {
    if (activeItem && activeItem.id !== item) {
      activeItem.isActive = false;
    }
    activeItem = { id: item, isActive: true };
  }
</script>

<!-- 
    - #HEADER
  -->

<header class="header" data-header>
  <a href="/" class="logo">
    <img
      src="media/logo-light.svg"
      width="156"
      height="32"
      alt="Cook.io"
      class="logo-light"
    />
    <img
      src="media/logo-dark.svg"
      width="156"
      height="32"
      alt="Cook.io"
      class="logo-dark"
    />
  </a>

  <nav class="navbar">
    <ul class="navbar-list">
      <li on:click={() => setActive("home")}>
        <a
          href="/"
          class="navbar-link title-small has-state {activeItem.id === 'home'
            ? 'active'
            : ''}">Home</a
        >
      </li>

      <li on:click={() => setActive("recipes")}>
        <a
          href="recipes"
          class="navbar-link title-small has-state {activeItem.id === 'recipes'
            ? 'active'
            : ''}">Recipes</a
        >
      </li>
    </ul>
  </nav>

  <button
    class="icon-btn theme-switch has-state"
    aria-pressed="false"
    aria-label="Toggle light and dark theme"
    data-theme-btn
  >
    <span class="material-symbols-outlined light-icon" aria-hidden="true"
      >light_mode</span
    >

    <span class="material-symbols-outlined dark-icon" aria-hidden="true"
      >dark_mode</span
    >
  </button>

  <a href="saved-recipes" class="btn btn-primary has-icon">
    <span class="material-symbols-outlined" aria-hidden="true">book</span>

    <span class="span">Saved Recipes</span>
  </a>
</header>
