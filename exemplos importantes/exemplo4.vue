<!DOCTYPE html>
<html lang="pt-br">
<head>
	<meta charset="utf-8">
	<title>Teste vueJS</title>
</head>
<body>
	<div id="app">
		<h1>{{ titulo }}</h1>
		<label for="">Nome</label><br>
		<input type="text" v-model="nome">

		<br><br>
		<label for="">Telefone</label><br>
		<input type="text" v-model="telefone">

		<br><br>
		<label for="">Deseja receber novidades?</label><br>
		<input type="radio" value="sim" v-model="novidades"> Sim
		<input type="radio" value="não" v-model="novidades"> Não

		<br><br>
		<label for="">Interesses</label><br>
		<input type="checkbox" value="Futebol" v-model="interesses"> Futebol <br>
		<input type="checkbox" value="Fórmula 1" v-model="interesses"> Fórmula 1 <br>
		<input type="checkbox" value="Vôlei" v-model="interesses"> Vôlei <br>
		
		<br><br>
		<label for="">Como nos conheceu?</label><br>
		<select v-model="conheceu">
			<option value="">Escolha</option>
			<option value="Google">Google</option>
			<option value="TV">TV</option>
			<option value="Revista">Revista</option>
		</select>

		<br><br>
		<button>ENVIAR</button>

		<br><br><br>
		<!-- MOSTRAR AS INFORMAÇÕES NA TELA DO USUÁRIO
		Nome: {{nome}} <br>
		Telefone: {{telefone}} <br>
		Novidades: {{novidades}} <br>
		Interesses: {{interesses}} <br>
		Como nos conheceu? {{conheceu}} <br>
		-->
	</div>

	<script src="https://cdn.jsdelivr.net/npm/vue"></script>

	<script>
		var app = new Vue({
			el: "#app", /* elemento */
			data: { /* local de armazenamento de variáveis */
				titulo: "Aulas - VueJs",
				nome: "",
				telefone: "",
				novidades: "",
				interesses: [],
				conheceu: "",
			}
		});
	</script>
</body>
</html>