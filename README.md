# paginawebcielo.github.io
<script>
  var obj = {pDouble: 1.99, pString: 'parâmetros', pInt: 2, pBoolean: true}
  var str = JSON.stringify(obj);
</script>
<button style="background-color: yellow;" type="button" onclick="native.navigateToNativeFlow('APP_ANDROID_PIX', null, false);">Abrir tela nativa sem parâmetros</button><br/>
<button style="background-color: lightblue;" type="button" onclick="native.navigateToNativeFlow('APP_ANDROID_PIX', str, true);">Abrir tela nativa com parâmetros</button><br/>
