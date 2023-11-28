<script>
  import Footer from "./footer.svelte";
  import Head from "./head.svelte";
  import Header from "./header.svelte";
  import Nav from "./nav.svelte";

  export let content, layout, allContent, allLayouts;
</script>

<html lang="en" data-theme="dark">
  <Head />
  <body>
    <Header />
    <Nav />
    <main>
      <article>
        <svelte:component
          this={layout}
          {...content.fields}
          {allContent}
          {allLayouts}
          {content}
        />
      </article>
    </main>
    <Footer />
  </body>
</html>
