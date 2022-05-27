# imc
Código para calcular IMC
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>IMC</title>
</head>
<body>
	
</body>
</html>

<script>

    function pulaLinha() {

        document.write("<BR><BR>");

    }

    function mostra(frase) {

        document.write(frase);
        pulaLinha();

    }

        function calculaImc(altura, peso) {

            return peso / (altura * altura);
            
        }
        
        var nome = prompt("Informe o seu nome");
        var alturaInformada = prompt(nome + ", informe sua altura ");
        var pesoInformado = prompt(nome + ", informe o seu peso ");
        
        var imc = calculaImc(alturaInformada, pesoInformado);

        mostra(nome + " o seu IMC calculado é " + imc);

        if(imc < 18.5) {

            mostra("Você está abaixo do recomendado ")

        }

        if(imc > 35){

            mostra("Você está acima do recomendado");

        }

        if (imc >=18.5 && imc <=35){

            mostra("Seu IMC está excelente!");

        }



</script>
