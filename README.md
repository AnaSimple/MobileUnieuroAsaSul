6) Fazer uma função para identificar se a palavra digitada pelo usuário é um
palíndromo ou não. Uma palavra é denominada um palíndromo se for invertida e
a leitura da mesma permanecer sem nenhuma alteração. Ex.: aba, radar, reter, rever, rir. Após criada, chame a função usando eventos.


<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Exerc. 6</title>
</head>
<body id="content">
    <h3>
        6) Fazer uma função para identificar se a palavra digitada pelo usuário é um
        palíndromo ou não. Uma palavra é denominada um palíndromo se for invertida e
        a leitura da mesma permanecer sem nenhuma alteração. Ex.: aba, radar, reter, rever, rir. Após criada, chame a função usando eventos.
    </h3>

    <input type="text" id="palavra">
    <button onclick="verificaPolindromo(document.getElementById('palavra').value)">Verifica políndromo</button>

    <script src="scripts.js"></script>
    <script>
        function verificaPolindromo(palavra) {
            let palavraInvertida = palavra.split("").reverse().join("");
            if(palavraInvertida === palavra){
                alert("É POLINDROMO");
            } else {
                alert("Não é polindromo :(");
            }
        }
    </script>
</body>
</html>
