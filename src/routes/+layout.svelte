<script>
  import "../app.css"
  import Navbar from "../components/navbar.svelte";
  import Footer from "../components/footer.svelte";
</script>

<div class="background">
  <Navbar />
  <slot> </slot>
  <Footer />
</div>


<style>

</style>
