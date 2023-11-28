<!-- 
        - #TAB
      -->

<section class="section tab">
  <div class="container">
    <div class="tab-list" data-tab-list role="tablist" aria-label="Meal type">
      <button
        class="tab-btn title-small"
        role="tab"
        id="tab-1"
        tabindex="0"
        aria-controls="panel-1"
        aria-selected="true"
        data-tab-btn>Breakfast</button
      >

      <button
        class="tab-btn title-small"
        role="tab"
        id="tab-2"
        tabindex="-1"
        aria-controls="panel-2"
        aria-selected="false"
        data-tab-btn>Lunch</button
      >

      <button
        class="tab-btn title-small"
        role="tab"
        id="tab-3"
        tabindex="-1"
        aria-controls="panel-3"
        aria-selected="false"
        data-tab-btn>Dinner</button
      >

      <button
        class="tab-btn title-small"
        role="tab"
        id="tab-4"
        tabindex="-1"
        aria-controls="panel-4"
        aria-selected="false"
        data-tab-btn>Snack</button
      >

      <button
        class="tab-btn title-small"
        role="tab"
        id="tab-5"
        tabindex="-1"
        aria-controls="panel-5"
        aria-selected="false"
        data-tab-btn>Teatime</button
      >
    </div>

    <div
      class="tab-panel"
      role="tabpanel"
      id="panel-1"
      aria-labelledby="tab-1"
      tabindex="0"
      data-tab-panel
    ></div>

    <div
      class="tab-panel"
      role="tabpanel"
      id="panel-2"
      aria-labelledby="tab-2"
      tabindex="0"
      data-tab-panel
      hidden
    >
      Lunch
    </div>

    <div
      class="tab-panel"
      role="tabpanel"
      id="panel-3"
      aria-labelledby="tab-3"
      tabindex="0"
      data-tab-panel
      hidden
    >
      Dinner
    </div>

    <div
      class="tab-panel"
      role="tabpanel"
      id="panel-4"
      aria-labelledby="tab-4"
      tabindex="0"
      data-tab-panel
      hidden
    >
      Snack
    </div>

    <div
      class="tab-panel"
      role="tabpanel"
      id="panel-5"
      aria-labelledby="tab-5"
      tabindex="0"
      data-tab-panel
      hidden
    >
      Teatime
    </div>
  </div>
</section>
