<!DOCTYPE html>
<html lang="pt-br">
<head>
	<meta charset="utf-8">
	<title>Teste vueJS</title>
</head>
<body>
	<div id="app">
		<h1 v-once>{{ titulo }}</h1>
		<img v-bind:src="imagem" width="450px">
	</div>

	<script src="https://cdn.jsdelivr.net/npm/vue"></script>

	<script>
		var app = new Vue({
			el: "#app", /* elemento */
			data: { /* local de armazenamento de variáveis */
				titulo: "Aulas - VueJs",
				imagem: "http://cdn.vs.com.br/vs-img/1526479533835-league-of-legendsss.jpg",
			}
		});
	</script>
</body>
</html>