<script>
	let counter = 0

	const modifyCounter = (n)=> counter+=n

	const reset = ()=> counter = 0

</script>

<main>
	<h1 class="text-center">Counter APP</h1>
	<hr>
  	<h2>Counter: <span class={counter < 0 ? "negative" : "positive"}>{counter}</span></h2>
	<button on:click={ ()=> {modifyCounter(1)} }>+1</button>
	<button on:click={ ()=> {modifyCounter(-1)} }>-1</button>
	<button on:click={ reset }>reset</button>
</main>

<!--  HTML PARA EL CRUD
	<div class="container mt-5">
		<div class="row">
			<div class="col-12 text-center">
				<h1 class="text-danger">CRUD CON SVELTE</h1>
			</div>
		</div>

		<div class="row justify-content-center mt-5">
			<div class="col-8">
				<form action="" method="POST">
					<div class="input-group mb-3">
						<input type="text" class="form-control" placeholder="Agregar tarea" aria-label="Agregar tarea" aria-describedby="Entrada de texto">
						<button class="btn btn-success" type="submit" id="button-addon1">Guardar</button>
					</div>
				</form>
			</div>
		</div>
	</div> -->
<style>

.negative
{
	color: red;
}

.positive
{
	color: greenyellow;
}

</style>
