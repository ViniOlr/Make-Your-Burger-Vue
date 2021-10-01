<template>
	<div id="nav">
		<div class="container">
			<rounter-link to="/" class="logo_url">
				<img :src="logo" :alt="alt" id="logo">
			</rounter-link>
			<router-link to="/">Home</router-link> |
			<router-link to="/pedidos">Pedidos</router-link>
		</div>
	</div>
</template>

<script>
export default {
  name: "NavBar",
	props: ["logo", "alt","permissao"]
}
</script>

<style scoped>
  #nav {
    background-color: var(--background);
    border-bottom: 4px solid var(--border);
    padding: 5px 50px;
  }
  #nav > .container {
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  #nav .logo_url {
    margin: auto;
    margin-left: 0;
  }
  #logo {
    width: 75px;
  }
  #nav a {
    color: var(--font);
    text-decoration: none;
    margin: 12px;
    transition: .5s;
    font-size: 1.3em;
  }
  #nav a:hover {
    color: white;
  }
</style>