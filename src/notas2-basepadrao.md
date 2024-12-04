
<!--  notas invisiveis -->

01 Passo - html base padrao para inicializar a criacao dea pagina.
-------------------------------------------------------

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Memory-Game-WASh</title>
    <link rel="stylesheet" href="./src/styles/reset.css">
    <link rel="stylesheet" href="./src/styles/main.css">
</head>
<body>
    <!-- // div.container>(h2+div+button) -->
    <div class="container">
        <h2>Memory-Game-WaSh</h2>
        <div class="game"></div>
        <button class="reset" onclick="window.Location.reload()">RESET GAME</button>
    </div>


    <script src="./src/scripts/engine.js" defer></script>

</body>
</html>

02 Passo -----------implementando o "styles/reset.css"--------------------
Obijetivo e padronizar o nosso html com todos os navegadores.

* {
    margin: 0;
    padding: 0;
    outline: none;
    box-sizing: border-box;
    font-family: monospace;
}

03 Passo ------ Configurar o Body do nosso html no "styles/main.css" -----

body {
    display: flex;  <!-- display unico- usado para quando nao tem muitos elementos -->
    justify-content: center;  <!-- Justificado ao centro na horizontal -->
    align-items: center;      <!-- alinhado ao centro na vertical -->
    min-height: 100vh;         <!-- definir que quero 100 % da pagina do html -->
    background: #763892;      <!-- define a Cor do Back ground -->
}

04 passo ----- personalizar ao nosso "container" no "main.css"----------------

Que esta no "Body" do nosso "index.html" ==> <div class="container">

Que contem O texto " <h2>Memory-Game-WaSh</h2> " e o botao " reset game " 
" <button class="reset" onclick="window.Location.reload()">RESET GAME</button> "

.container{
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 30px;             <!-- Define uma distancia entre os elementos de 30px -->
    background: linear-gradient(325deg, #03001e 0%, #7303c0 30%, #ec38bc 70%, #fdeff9 100%);
    padding: 40px 60px;     <!--Enxima e embaixo 40px,  dnos lados 60px -->
}

05 Passo --- Estilizando o nosso "Texto" <h2>Memory-Game-WaSh</h2> no main.css----
    
h2{
    font-size: 3em;
    color: #fff;
    text-transform: uppercase;       <!-- define letras em Maiusculo>
    letter-spacing: 0.1em;          <!-- Espacamento entre as letras >

}

06 Passo ----- Estilizando  o "botao do Reset" - no main.css-------

.reset

.reset {
    padding: 15px 20px;
    width: 100%;
    color: #03001e;
    background-color: #fff;
    border: #ec38bc;
    border-radius: 20px;
    font-size: 1.5em;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    cursor: pointer;
    font-weight: 600;

}

07 Passo ----Estilizando um "refrech" no botao "Reset"
.reset:focus {
    color: #ec38bc;
    background-color: #262809;
    
}

08 passo -- Estilizando a "div Games" -- <div class="game"></div> -- no main.css --

.game{
    border: 1px solid red;
    width: 430px;
    height: 430px;
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    transform-style: preserve-3d;
    perspective: 500px;
}

09 Passo -- Estilizando " .item  "  no main.css -----------
---  que sera ainda criada. 

.item {
    position: relative;
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #fdeff9;
}








