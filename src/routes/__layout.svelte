<script>
  import '../app.css'
  import Header from '$lib/components/header.svelte'
  import Footer from '$lib/components/footer.svelte'
	import Slider from '$lib/components/slider.svelte';
  import Navbar from '$lib/components/navbar.svelte';
  import Servicios from '$lib/components/Servicios.svelte';
  import NuestrosTrabajos from '$lib/components/NuestrosTrabajos.svelte';
  import QuienesSomos from '$lib/components/QuienesSomos.svelte';
  import Slogan from '$lib/components/Slogan.svelte';
  import QueDicenNuestrosClientes from '$lib/components/QueDicenNuestrosClientes.svelte';
  import NuestrosClientes from '$lib/components/NuestrosClientes.svelte';
  import Cursos from '$lib/components/Cursos.svelte';
  import Newsletter from '$lib/components/Newsletter.svelte';
  import Contactanos from '$lib/components/Contactanos.svelte';
</script>

<main>
  <Navbar></Navbar>
  <Slider></Slider>
  <Servicios></Servicios> 
  <NuestrosTrabajos></NuestrosTrabajos>
  <QuienesSomos></QuienesSomos>
  <Slogan></Slogan>
  <QueDicenNuestrosClientes></QueDicenNuestrosClientes>
  <NuestrosClientes></NuestrosClientes>
  <Newsletter></Newsletter>
  <Cursos></Cursos>
  <Contactanos></Contactanos>
  <Footer></Footer>
</main>




