<!DOCTYPE html>
<html>
<head>
	<title>Teste vueJS</title>
</head>
<body>
	<div id="app">
		<h1>{{ titulo }}</h1>
		<p v-if="status">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
		quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
		cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
		proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
		
		<p v-else>Não tem texto aqui!</p>
	</div>

	<script src="https://cdn.jsdelivr.net/npm/vue"></script>

	<script>
		var app = new Vue({
			el: "#app", /* elemento */
			data: { /* local de armazenamento de variáveis */
				status: false,
				titulo: "Aula 01 - VueJs"
			}

		});
	</script>
</body>
</html>