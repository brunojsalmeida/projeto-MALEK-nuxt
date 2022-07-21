<template>
    <div>
        <p class="subtitulo">Minhas informações</p>
        <br>

    <form class="mt-5">
        <fieldset class="d-flex gap-1">
            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Nome *</label>
                <input type="text" class="form-control" id="nome" placeholder="João">
            </div>

            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Sobrenome *</label>
                <input type="text" class="form-control" id="sobrenome" placeholder="Souza">
            </div>
        </fieldset>

        <div class="mb-3 col-12">
            <label for="form-control" class="form-label">CPF/CNPJ *</label>
            <input type="text" class="form-control" id="cfp/cnpj" placeholder="000.000.000-00">
        </div>

        <div class="mb-3 col-12">
            <label for="form-control" class="form-label">Email *</label>
            <input type="email" class="form-control" id="email" placeholder="name@example.com">
          </div>

          <div class="d-flex gap-1">
            <div class="form-group col-3">
                <label for="ddd">DDD *</label>
                <input type="text" class="form-control" id="DDD" placeholder="00">
              </div>
    
              <div class="form-group col-9">
                <label for="tel">Telefone *</label>
                <input type="text" class="form-control" id="tel" placeholder="00000-0000">
              </div>
          </div>

        <fieldset class="d-flex gap-1">
            <div class="mb-3 col-6 mt-3">
                <label for="form-control" class="form-label">CEP *</label>
                <input type="number" class="form-control" id="cep" placeholder="00-000000">
            </div>

            <div class="mb-3 col-6 mt-3">
                <label for="form-control" class="form-label">Bairro</label>
                <input type="text" class="form-control" id="bairro" placeholder="-">
            </div>
        </fieldset>
        <fieldset class="d-flex gap-1">
            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Cidade</label>
                <input type="text" class="form-control" id="cidade" placeholder="-">
            </div>

            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Estado</label>
                <input type="text" class="form-control" id="estado" placeholder="-">
            </div>
        </fieldset>
        <fieldset class="d-flex gap-1">
            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Número</label>
                <input type="number" class="form-control" id="numero" placeholder="-">
            </div>

            <div class="mb-3 col-6">
                <label for="form-control" class="form-label">Complemento</label>
                <input type="text" class="form-control" id="complemento" placeholder="-">
            </div>
        </fieldset>

        <button class="botao" type="submit">Avançar</button>
    </form>


    </div>

</template>

<script>

export default {
    layout: 'form',

}
</script>

<style>

label{
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 150%;



    color: #5B5B5B;
}

form {
    width: 100%;
}
</style>