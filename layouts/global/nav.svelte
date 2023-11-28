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
    - #MOBILE NAV
  -->

<nav class="mobile-nav" aria-label="primary">
  <ul class="nav-list">
    <li class="nav-item">
      <a href="recipes" class="nav-link">
        <span class="item-icon">
          <span class="material-symbols-outlined" aria-hidden="true"
            >lunch_dining</span
          >
        </span>

        <span class="label-medium">Recipes</span>
      </a>
    </li>

    <li class="nav-item">
      <a href="/" class="nav-link" aria-current="true">
        <span class="item-icon">
          <span class="material-symbols-outlined" aria-hidden="true">home</span>
        </span>

        <span class="label-medium">Home</span>
      </a>
    </li>

    <li class="nav-item">
      <a href="saved-recipes" class="nav-link">
        <span class="item-icon">
          <span class="material-symbols-outlined" aria-hidden="true">book</span>
        </span>

        <span class="label-medium">Saved</span>
      </a>
    </li>
  </ul>
</nav>
