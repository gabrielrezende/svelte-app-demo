<script>
	import CreateUserForm from "./CreateUserForm.svelte";
</script>

<div class="container">
	<div class="container-lado container-lado-esquerdo">
		<p>
			Welcome to your professional gaming community
		</p>
	</div>
	<div class="container-lado">
		<p class="titulo-plataforma">
			Allamo PRO
		</p>
		<div class="formulario">
			<CreateUserForm>

			</CreateUserForm>
		</div>
		<a href="/criar-conta" class="botao-criar-conta">
			Criar conta
		</a>
	</div>
</div>

<style>
	.container{
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: row;
	}
	.container-lado{
		width: 50%;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		/*justify-content: center;*/
	}
	.container-lado.container-lado-esquerdo{
		border-right: #333333 1px solid;
	}
	.container-lado p{
		font-size: 24px;
		font-weight: bold;
	}
	.titulo-plataforma{
		font-size: 40px !important;
	}
	.formulario{
		height: 100%;
		width: 400px;
		max-width: 500px;
		padding: 10px;
		display: flex;
		flex-direction: row;
		align-items: flex-end;
	}
	.botao-criar-conta{
		margin: 20px;
	}
</style>