<template>
  <div>
    <p class="subtitulo">Minha marca</p>
        <br>

    <label class="picture" for="picture__input" tabindex="0">
    <input type="file" accept="image/*" class="picture__input" />
    <div class="container">
        <img class="pb-4" src="~assets/upload.svg" alt="Upload">
        <span class="picture__image">Clique para enviar sua logo</span>
        <span class="legenda">PNG, JPG (tamanho máximo X)</span>
    </div>
    </label>

    <div class="container-2">
        <button class="botao-outline" type="button">Salvar</button>

        <button class="botao" type="submit">Avançar</button>
    </div>

  </div>
</template>

<script>
/*
    const inputFile = document.querySelector('#picture__input');
    const pictureImage = document.querySelector('.picture__image');
    const pictureImageTxt = "Clique para enviar sua logo";
    pictureImage.innerHTML = pictureImageTxt;

    inputFile.addEventListener('change', function(e){
        const inputTarget = e.target;
        const file = inputTarget.files[0];

        if(file) {
            const reader = new FileReader();

            reader.addEventListener('load', function(e){
                const readerTarget = e.target;

                const img = document.createElement('img');
                img.src = readerTarget.result;
                img.classList.add('picture__img');
                
                pictureImage.innerHTML = '';

                pictureImage.appendChild(img);
            });

            reader.readAsDataURL(file);
        } else {
            pictureImage.innerHTML = pictureImageTxt;
        }
    });
*/
export default {
    layout: 'form',
}
</script>

<style>

.picture__input{
    display: none;
}

.container{
    display: flex;
    flex-direction: column;
    gap: 10px;
    align-items: center;
}

.container-2{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
}

.picture{
    width: 319px;
    height: 210px;
    margin-top: 62px;
    cursor: pointer;

    display: flex;
    align-items: center;
    justify-content: center;

    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 150%;
    text-decoration-line: underline;
    color: #6B6E84;

    background: #FFFFFF;
    border-radius: 25px;
}

.legenda{
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 150%;

    color: #6B6E84;
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
    
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 20px;
    line-height: 150%;
    color: #002554;

    margin-top: 20px;
    margin-bottom: 50px;
}

</style>