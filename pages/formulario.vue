<template>
    <div>
        <p class="subtitulo">Minhas informações</p>
        <br>

    <form>
        <fieldset class="d-flex gap-2">
            <div class="mb-3 col-5">
                <label for="form-control" class="form-label">Nome *</label>
                <input type="text" class="form-control" id="nome" placeholder="João">
            </div>

            <div class="mb-3 col-5">
                <label for="form-control" class="form-label">Sobrenome *</label>
                <input type="text" class="form-control" id="sobrenome" placeholder="Souza">
            </div>
        </fieldset>

        <div class="mb-3 col-10">
            <label for="form-control" class="form-label">CPF/CNPJ *</label>
            <input type="text" class="form-control" id="cfp/cnpj" placeholder="000.000.000-00">
        </div>

        <div class="mb-3 col-10">
            <label for="form-control" class="form-label">Email *</label>
            <input type="email" class="form-control" id="email" placeholder="name@example.com">
          </div>

          <div class="d-flex gap-2">
            <div class="form-group col-2">
                <label for="ddd">DDD *</label>
                <input type="text" class="form-control" id="ddd" placeholder="00">
              </div>
    
              <div class="form-group col-7">
                <label for="tel">Telefone *</label>
                <input type="text" class="form-control" id="tel" placeholder="00000-0000">
              </div>
          </div>

        <fieldset class="d-flex gap-2 flex-wrap">
            <div class="mb-3 col-5 mt-3">
                <label for="form-control" class="form-label">CEP *</label>
                <input type="number" class="form-control" id="cep" placeholder="00-000000">
            </div>

            <div class="mb-3 col-5 mt-3">
                <label for="form-control" class="form-label">Bairro</label>
                <input type="text" class="form-control" id="bairro" placeholder="-">
            </div>

            <div class="mb-3 col-5">
                <label for="form-control" class="form-label">Cidade</label>
                <input type="text" class="form-control" id="cidade" placeholder="-">
            </div>

            <div class="mb-3 col-5">
                <label for="form-control" class="form-label">Estado</label>
                <input type="text" class="form-control" id="estado" placeholder="-">
            </div>

            <div class="mb-3 col-5">
                <label for="form-control" class="form-label">Número</label>
                <input type="number" class="form-control" id="numero" placeholder="-">
            </div>

            <div class="mb-3 col-5">
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
    font-family: 'Popins';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 150%;



    color: #5B5B5B;
}

.botao{
    font-size: 1.2em;
    background: #000066;
    box-shadow: 0px 4px 4px rgba(0, 71, 187, 0.06);
    border-radius: 8px;
    padding: 8px 114px 8px 115px;
    border: 0;
    color: #FFFFFF;
    margin-top: 20px;
    margin-bottom: 23px;
}

.botao:hover {
    background: #ccbbff;
    box-shadow: inset 2px 2px 2px rgba(0, 0, 0, 0.2);
    text-shadow: none;
}

@media (max-width: 460px){

    .botao{
        width: 270px;
        padding-left: 100px;
    }

}
</style>