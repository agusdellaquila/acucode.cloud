<script>
  import "../app.css"
</script>

<div class="background">
  <slot> </slot>
</div>


<style>
	.background {
		background: linear-gradient(180deg, #82ADDB 0%, #757ABF 54.17%, #191621 100%);
		color: white;
		height: 100vh;
		margin: 0rem;
		overflow: hidden; 
	}
</style>
