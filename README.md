<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animação Simples</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Meu Projeto Animado no GitHub</h1>
    </header>

    <div class="quadrado-animado"></div>

    <p>Este é um exemplo simples de animação CSS.</p>

</body>
</html>

/* Estilização básica para o corpo da página */
body {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    margin: 0;
    font-family: sans-serif;
    background-color: #f0f0f0;
}

h1 {
    color: #333;
    margin-bottom: 30px;
}

/* Estilização inicial do elemento a ser animado */
.quadrado-animado {
    width: 100px;
    height: 100px;
    background-color: dodgerblue; /* Cor inicial */
    border-radius: 10px;
    /* Aplica a animação: nome, duração, repetição, função de tempo */
    animation: moverCor 4s infinite alternate ease-in-out;
}

/* @keyframes define o ciclo da animação.
   Aqui, a animação é chamada 'moverCor'.
*/
@keyframes moverCor {
    /* 0% (início da animação) */
    0% {
        transform: translateX(-150px) rotate(0deg); /* Posição inicial (para a esquerda) e sem rotação */
        background-color: dodgerblue;
    }

    /* 50% (meio da animação) */
    50% {
        background-color: tomato; /* Muda a cor no meio do movimento */
    }

    /* 100% (fim da animação) */
    100% {
        transform: translateX(150px) rotate(360deg); /* Posição final (para a direita) e rotação completa */
        background-color: seagreen;
    }
}
<!--
**duarteescola877-creator/duarteescola877-creator** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
