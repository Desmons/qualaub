<script>
  import { goto } from "$app/navigation";

	let open = false
	function handleOpen() {
		open = !open
	}
</script>

<nav>
	<div class="logo">
		<img src="/images/qualaub.jpg" alt="qualaub logo">
	</div>
	<div class="hamburger" class:open={open} class:toggle={open} on:click={handleOpen}>
		<div class="line1"></div>
		<div class="line2"></div>
		<div class="line3"></div>
	</div>
	<ul class="nav-links" class:open={open}>
		<li class:fade={open}><a href="/" class="title">Inicio</a></li>
    <li class:fade={open}><a href="/" class="title">Quiénes somos</a></li>
		<li class:fade={open}><a href="/" class="title">Nuestros Servicios</a></li>
		<li class:fade={open}><a href="/" class="title">Contáctenos</a></li>
    <li class:fade={open}>
      <div class="lang-container">
        <select class="language">
          <option value="es">🇪🇸</option>
          <option value="en">🇬🇧</option>
        </select>
      </div>
    </li>
	</ul>
</nav>

<style>
  nav {
    height: 6rem;
    width: 100%;
    background-color: #a0a0a0;
    box-shadow: 0 3px 20px rgba(0, 0, 0, 0.3);
    display: flex;
    position: fixed;
    z-index: 10;
  }
  /*Styling logo*/
  .logo {
    padding-left: 40px;
    text-align: center;
  }
  .logo img {
    height: 96px;
    width: auto;
  }
  /*Styling Links*/
  .nav-links {
    display: flex;
    list-style: none; 
    width: 88vw;
    padding: 0 0.7vw;
    margin-right: 40px;
    margin-top: 14px;
    justify-content: right;
    align-items: center;
    text-transform: uppercase;
  }
  .nav-links li a {
    text-decoration: none;
    margin: 20px
  }
  .nav-links li a:hover {
    color: #fbe07e;
  }
  .nav-links li {
    position: relative;
  }
  .nav-links li a::before {
    content: "";
    display: block;
    height: 3px;
    width: 0%;
    background-color: #FEC701;
    position: absolute;
    transition: all ease-in-out 250ms;
    margin: 0 0 0 10%;
  }
  .nav-links li a:hover::before{
    width: 80%;
  }

  /*Styling Hamburger Icon*/
  .hamburger div{
    width: 30px;
    height: 3px;
    background: #FEC701;
    margin: 5px;
    transition: all 0.3s ease;
  }
  .hamburger{
    display: none;
  }

  /* select language */
  .lang-container {
    margin-top: -8px
  }
  .language {
    border: none;
    font-size: 30px;
    margin-top: 6px;
    background-color: #a0a0a0;
    outline: 0;
  }
  .language:hover {
    cursor: pointer;
  }


  /*Stying for small screens*/
  @media screen and (max-width: 800px){
    nav{
      position: fixed;
      z-index: 3;
    }
    .hamburger{
      display:block;
      position: absolute;
      cursor: pointer;
      right: 5%;
      top: 50%;
      transform: translate(-5%, -50%);
      z-index: 2;
      transition: all 0.7s ease;
    }
    .nav-links{
      position: fixed;
      background: #a0a0a0;
      height: 100vh;
      width: 100%;
      margin-top: 0;
      flex-direction: column;
      clip-path: circle(50px at 90% -20%);
      -webkit-clip-path: circle(50px at 90% -10%);
      transition: all 1s ease-out;
      pointer-events: none;
    }
    .nav-links.open{
      clip-path: circle(1000px at 90% -10%);
      -webkit-clip-path: circle(1000px at 90% -10%);
      pointer-events: all;
    }
    .nav-links li{
      opacity: 0;
    }
    .nav-links li:nth-child(1){
      transition: all 0.5s ease 0.2s;
    }
    .nav-links li:nth-child(2){
      transition: all 0.5s ease 0.4s;
    }
    .nav-links li:nth-child(3){
      transition: all 0.5s ease 0.6s;
    }
    .nav-links li:nth-child(4){
      transition: all 0.5s ease 0.7s;
    }
    .nav-links li:nth-child(5){
      transition: all 0.5s ease 0.8s;
    }
    .nav-links li:nth-child(6){
      transition: all 0.5s ease 0.9s;
      margin: 0;
    }
    .nav-links li:nth-child(7){
      transition: all 0.5s ease 1s;
      margin: 0;
    }
    li.fade{
      opacity: 1;
    }
  }
  /*Animating Hamburger Icon on Click*/
  .toggle .line1{
    transform: rotate(-45deg) translate(-5px,6px);
  }
  .toggle .line2{
    transition: all 0.7s ease;
    width: 0;
  }
  .toggle .line3{
    transform: rotate(45deg) translate(-5px,-6px);
  }
</style>