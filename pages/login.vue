<template>
    <div>
        <img class="logo" src="~assets/logo.svg" alt="Logo ACME">

        <form class="campo-login">

            <InputEmail > E-mail ou CPF / CNPJ </InputEmail>

            <div class="form-group mb-3 col-12">
                <label class="senha">Senha</label>
                <input type="password" class="form-control" id="exampleInputPassword1" placeholder="********">
            </div>

        </form>

        <div class="form-check d-flex flex-row justify-content-between">
                <div>
                    <input type="checkbox" class="form-check-input" id="exampleCheck1">
                    <label class="form-check-label" for="exampleCheck1" style="font-size: 12px; font-weight: 400; font-style: normal; line-height: 150%; color: #5B5B5B;">Lembrar senha</label>
                </div>
                <div>
                    <span class="text-decoration-underline" style="font-size: 12px; font-weight: 400; font-style: normal; line-height: 150%; color: #5B5B5B;">Esqueci minha senha</span>
                </div>
            </div>
        
            <SubmitButton class="mt-5" > Entrar </SubmitButton>
    </div>
</template>

<script>
export default {
    layout: 'defaut',

}
</script>

<style>


.logo{
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-top: 111px;
}

.campo-login{
    margin-top: 70px;
}

.senha{
    font-style: Medium;
    font-size: 12px;
    line-height: 18px;
    line-height: 150%;
    align: Left;
    vertical-align: Top;
    color: #5B5B5B;
}

</style>