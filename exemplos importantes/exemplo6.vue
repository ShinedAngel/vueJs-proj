<script src="https://cdn.jsdelivr.net/npm/vue"></script>

	<div id="app">
		<h1></h1>
		<button v-on:click="somar(5, $event)">São {{ contador }} cliques até agora</button>
		<p v-on:mousemove="atualizarXY">Mouse: {{ x }} e {{ y }}</p>
		<span v-on:mousemove="parar">PARAR AQUI!</span>
	</div>

	<script>
		var app = new Vue({
			el: "#app", /* elemento */
			data: { /* local de armazena  mento de variáveis */
				contador: 0,
				x: 0,
				y: 0,	
			},
			methods: { 
				somar(passo){
					console.log(passo, event),
					this.contador += passo
				},
				atualizarXY(event) {
					this.x = event.clientX
					this.y = event.clientY
				},
				parar(event) {
					event.stopPropagation()
				}
			}
		});
	</script>