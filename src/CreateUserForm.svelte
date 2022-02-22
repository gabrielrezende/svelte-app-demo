<script>
    import Input from "./Input.svelte";
    import Button from "./Button.svelte";

    const onClickFacebook = () => {
        console.log('facebook');
    }

    const onClickGoogle = () => {
        console.log('google');
    }

    const onClickEntrar = () =>{
        console.log('entra');
    }

    const onClickLinkedin = () =>{
        console.log('linkedin');
    }
</script>

<div class="container">
    <Input type="text" placeholder="Digite o seu e-mail" />
    <Input type="text" placeholder="Digite a sua senha" />
    <div class="container-botoes-de-acao">
        <a href="/esqueci-minha-senha"> Esqueci minha senha </a>
        <Button onClick={onClickEntrar}>
            Entrar
        </Button>
    </div>
    <p>OU</p>
    <Button width="100%" backgroundColor="#38548F" onClick={onClickFacebook}>
        Facebook
    </Button>
    <Button width="100%" backgroundColor="#C4402F" onClick={onClickGoogle} >
        Google
    </Button>
    <Button width="100%" backgroundColor="#0961B8" onClick={onClickLinkedin}>
        Linkedin
    </Button>
</div>

<style>
    .container{
        width: 100%;
        height: 80%;
        display: flex;
        flex-direction: column;
        margin-bottom: 30px;
    }
    .container-botoes-de-acao{
        width: 100%;
        height: 50px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }
    a{
        font-size: 12px;
    }
    p{
        text-align: center;
        font-size: 24px;
    }
</style>