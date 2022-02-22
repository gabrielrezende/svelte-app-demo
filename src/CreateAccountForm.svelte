<script>
    import Input from "./Input.svelte";
    import Button from "./ButtonAccount.svelte";

    const onClickFacebook = () => {
        console.log('facebook');
    }

    const onClickGoogle = () => {
        console.log('google');
    }

    const onClickCriarConta = () =>{
        console.log('criar');
    }

    const onClickLinkedin = () =>{
        console.log('linkedin');
    }
</script>

<div class="container">
    <Input type="text" placeholder="First Name" />
    <Input type="text" placeholder="Last Name" />
    <Input type="text" placeholder="Username" />
    <Input type="text" placeholder="Sexo" />
    <Input type="text" placeholder="Nascimento" />
    <Input type="text" placeholder="E-mail" />
    <Input type="text" placeholder="Senha" />
    <div class="container-botoes-de-acao">        
        <Button onClick={onClickCriarConta}>
            Criar Conta
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
        flex-direction: column;
    }    
    p{
        text-align: center;
        font-size: 24px;
    }
</style>