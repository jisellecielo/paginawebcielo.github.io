# paginawebcielo.github.io
<style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      max-width: 400px;
      margin: 0 auto;
    }
    input {
      width: 100%;
      padding: 10px;
      margin: 5px 0;
      box-sizing: border-box;
    }
    button {
      background-color: #4CAF50;
      color: white;
      padding: 15px 20px;
      border: none;
      cursor: pointer;
      width: 100%;
      margin: 10px 0;
    }
    button:hover {
      background-color: #45a049;
    }
    .mensagem-erro, .mensagem-sucesso {
      text-align: center;
      margin-top: 10px;
    }
    .mensagem-erro {
      color: red;
    }
    .mensagem-sucesso {
      color: green;
    }
    .example {
      font-size: 0.8em;
      color: #888;
    }
</style>
<script>
  //var obj = {pDouble: 1.99, pString: 'parâmetros', pInt: 2, pBoolean: true}
  //var str = JSON.stringify(obj);

  function enviarDados() {
      /*var cardBrandCode = document.getElementById('cardBrandCode').value;
      var authorizationCode = document.getElementById('authorizationCode').value;
      var nsu = document.getElementById('nsu').value;
      var truncatedCardNumber = document.getElementById('truncatedCardNumber').value;
      var authorizationDate = document.getElementById('authorizationDate').value;
      var paymentTypeCode = document.getElementById('paymentTypeCode').value;
      var grossAmount = document.getElementById('grossAmount').value;
      var saleMerchant = document.getElementById('saleMerchant').value;
      var mensagemErro = document.getElementById('mensagemErro');
      var mensagemSucesso = document.getElementById('mensagemSucesso');

      if (cardBrandCode && authorizationCode && nsu && truncatedCardNumber && authorizationDate && paymentTypeCode && grossAmount && saleMerchant) {
        // Todos os campos preenchidos, pode prosseguir com o envio dos dados
        mensagemSucesso.textContent = 'Dados enviados com sucesso!';
        mensagemErro.textContent = '';

        // Montar os parâmetros em formato JSON
        var params = {
          cardBrandCode: cardBrandCode,
          authorizationCode: authorizationCode,
          nsu: nsu,
          truncatedCardNumber: truncatedCardNumber,
          authorizationDate: authorizationDate,
          paymentTypeCode: paymentTypeCode,
          grossAmount: grossAmount,
          saleMerchant: saleMerchant
        };*/

        var params2 = {
          finalityId: null,
          startNewShare: true,
          flowId: null,
          URLOrigin: "https://jisellecielo.github.io/retorno.github.io/?origin=web"
        };

        // Converter o objeto em uma string JSON
        //var params = JSON.stringify(params);
        var GENERIC_FLOW_PARAMS = JSON.stringify(params2);

        // Chamar a função navigateToNativeFlow
        native.navigateToNativeFlow("APP_ANDROID_OPENFINANCE", GENERIC_FLOW_PARAMS, true);
      /*} else {
        // Caso algum campo não esteja preenchido, exibe uma mensagem de erro
        mensagemErro.textContent = 'Por favor, preencha todos os campos!';
        mensagemSucesso.textContent = '';
      }*/
    }
  
</script>


<body>
 <!-- <h1>Dados da Transação</h1>
  <label for="cardBrandCode">Card Brand Code: <span class="example"> (Exemplo: 3)</span></label>
  <input type="text" id="cardBrandCode"><br>
  <label for="authorizationCode">Authorization Code: <span class="example"> (Exemplo: 811780)</span></label>
  <input type="text" id="authorizationCode"><br>
  <label for="nsu">NSU: <span class="example"> (Exemplo: 167700)</span></label>
  <input type="text" id="nsu"><br>
  <label for="truncatedCardNumber">Truncated Card Number: <span class="example"> (Exemplo: 3005)</span></label>
  <input type="text" id="truncatedCardNumber"><br>
  <label for="authorizationDate">Authorization Date: <span class="example"> (Exemplo: 2024-08-09)</span></label>
  <input type="text" id="authorizationDate"><br>
  <label for="paymentTypeCode">Payment Type Code: <span class="example"> (Exemplo: 52)</span></label>
  <input type="text" id="paymentTypeCode"><br>
  <label for="grossAmount">Gross Amount: <span class="example"> (Exemplo: 55.0)</span></label>
  <input type="text" id="grossAmount"><br>
  <label for="saleMerchant">Sale Merchant: <span class="example"> (Exemplo: 2121212112)</span></label>
  <input type="text" id="saleMerchant"><br>-->
  <button onclick="enviarDados()">Enviar</button><p class="mensagem-erro" id="mensagemErro"></p><p class="mensagem-sucesso" id="mensagemSucesso"></p>
</body>
<!--<button style="background-color: yellow;" type="button" onclick="native.navigateToNativeFlow('APP_ANDROID_PIX', null, false);">Abrir tela nativa sem parâmetros</button><br/>
<button style="background-color: lightblue;" type="button" onclick="native.navigateToNativeFlow('APP_ANDROID_PIX', str, true);">Abrir tela nativa com parâmetros</button><br/>-->
