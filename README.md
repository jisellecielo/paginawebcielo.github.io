# paginawebcielo.github.io
<script>
  var obj = {pDouble: 1.99, pString: 'parametros', pInt: 2, pBoolean: true}
  var str = JSON.stringify(obj);
</script>
<button style="background-color: lightblue;" type="button" onclick="native.navigateToNativeFlow('1', str, false);">Abrir tela nativa com parâmetros</button><br/>
<button style="background-color: yellow;" type="button" onclick="native.navigateToNativeFlow('1', null, false);">Abrir tela nativa sem parâmetros</button><br/>
