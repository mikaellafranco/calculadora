# calculadora
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CALCULADORA</title>
</head>
<style>
body {
background-image: url("https://cdn.dicionariopopular.com/imagens/nazareconfusamatematica.gif")
}
</style>

  <span><font face= "verdana" color="pink" size="10"><center>Calculadora Power Ranger</center></span>
  <br>
  <form>
    <center><table bgcolor="#FFE4E1" border=1>
      <tr>
        <td colspan="4">
          <input type="number" name="numero" id="primeiroNumero">
        </td>
      </tr>
      <tr>
        <td colspan="4">
          <input type="number" name="numero" id="segundoNumero">
        </td>
      </tr>
      <tr>
        <td><input type="button" value="+" onclick="somar()"></td>
        <td><input type="button" value="-" onclick="subtrair()"></td>
        <td><input type="button" value="*" onclick="multiplicar()"></td>
        <td><input type="button" value="/" onclick="dividir()"></td>
      </tr>
      <tr>
        <td colspan="4">
          <input type="number" name="numero" id="resultado" readonly>
          <!-- <div id="resultado"> -->
        </td>
      </tr>
      </center>
    </table>
  </form>
  <script>

    function somar() {

      const primeiroNumero = document.getElementById("primeiroNumero");
      const segundoNumero = document.getElementById("segundoNumero");

      document.getElementById("resultado").value = 
      Number(primeiroNumero.value) 
      + 
      Number(segundoNumero.value);

      primeiroNumero.value="";
      segundoNumero.value="";
    }

    function subtrair() {
      document.getElementById("resultado").value = Number(document.getElementById("primeiroNumero").value) - Number(document.getElementById("segundoNumero").value);

      document.getElementById("primeiroNumero").value="";
      document.getElementById("segundoNumero").value="";
    }

    function multiplicar() {
      document.getElementById("resultado").value = Number(document.getElementById("primeiroNumero").value) * Number(document.getElementById("segundoNumero").value);

      document.getElementById("primeiroNumero").value="";
      document.getElementById("segundoNumero").value="";
    }

    function dividir() {
      document.getElementById("resultado").value = Number(document.getElementById("primeiroNumero").value) / Number(document.getElementById("segundoNumero").value);
      
      document.getElementById("primeiroNumero").value="";
      document.getElementById("segundoNumero").value="";

    }
    function limparDados(){
    inputResultado.value = "";
    calculo.primeiroValor = 0;
    calculo.segundoValor = 0;
    calculo.funcaoParaCalcular = null;
}
  </script>
</body>
</html>

 https://www.w3schools.com/code/tryit.asp?filename=GEZZO9SAXT31
