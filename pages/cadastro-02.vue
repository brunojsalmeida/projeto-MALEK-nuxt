<template>
  <div>
     <p class="subtitulo">Minha marca</p>
     <br>

    <label class="picture" for="picture__input" tabindex="0">
    <input type="file" accept="image/*" class="picture__input" />
    <div class="d-flex flex-column gap-2 align-items-center">
        <img class="pb-4" src="~assets/upload.svg" alt="Upload">
        <span class="text-decoration-underline">Clique para enviar sua logo</span>
        <span class="legenda">PNG, JPG (tamanho máximo X)</span>
    </div>
    </label>

    <div class="d-flex flex-column justify-content-between align-items-center">
        <button class="botao-outline" type="button">Salvar</button>


        
    </div>

    <SubmitButton v-b-modal.modal-1> Avançar </SubmitButton>

    <b-modal id="modal-1">
    <div class="d-flex flex-column gap-2 align-items-center">
            <img src="~assets/email.svg" alt="Message">
            <h3>Verifique seu e-mail</h3>
            <p>Foi encaminhado um email para <br> email@gmail.com</p>
            <br>
            <p class="text-decoration-underline">Clique aqui para realizar o LOGIN</p>
        </div>
    </b-modal>

 </div>

 
 </template>

<script>
export default {
    layout: 'form',

}
</script>

<style>

.picture__input{
    display: none;
}

.picture{
    width: 100%;
    height: 210px;
    margin-top: 62px;
    cursor: pointer;

    display: flex;
    align-items: center;
    justify-content: center;

    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 150%;
    color: #6B6E84;

    background: #FFFFFF;
    border-radius: 25px;
}

.legenda{
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 150%;
    text-decoration-line: none;

    color: #6B6E84;
}

h3{
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    line-height: 32px;
    text-align: center;
    color: #2E328C;
}

p{
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    text-align: center;
    color: #667085;
}

.picture__img {
  max-width: 100%;
}

.botao-outline{
    background: #ffffff;
    border: 1px solid #000066;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.06);
    border-radius: 8px;
    padding: 8px 125px 8px 125px;

    font-style: normal;
    font-weight: 600;
    font-size: 20px;
    line-height: 150%;
    color: #002554;

    margin-top: 20px;
    margin-bottom: 50px;

    width: 100%;
}

@media (max-width: 360px){
    .botao-outline{
        padding: 8px 70px 8px 70px;
    }
}

@media (max-width: 500px){
    .botao-outline{
        width: 100%;
    }

}


</style>