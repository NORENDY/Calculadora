# Calculadora
Operaciones Basicas
<!DOCTYPE HTML-->
<html>
<head>
<meta charset="UTF-8">
<link rel="stylesheet" href="css/jquery-ui.css">
<link rel="stylesheet" href="css/jquery.mobile-1.4.5.min.css">
<script type="text/javascript" src="js/jquery-ui.js"></script>
<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript" src="js/jquery.mobile-1.4.5.min.js"></script> 
<script>
    $(document).ready(function (){
    $("#btnSuma").click(function (){
    var n1=parseInt($("#num1").val());
     var n2=parseInt($("#num2").val());
      var resultado=$("#resultado");
      resultado.val(n1+n2);
    });
    $(document).ready(function (){
    $("#btnResta").click(function (){
    var n1=parseInt($("#num1").val());
     var n2=parseInt($("#num2").val());
      var resultado=$("#resultado");
      resultado.val(n1-n2);
    });
    $(document).ready(function (){
    $("#btnDiv").click(function (){
    var n1=parseInt($("#num1").val());
     var n2=parseInt($("#num2").val());
      var resultado=$("#resultado");
      resultado.val(n1/n2);
    });
</script>
<style type="text/css">
    p{
        text-align: center;
        
    }
</style>
</head>
<body>
    <div data-role="page" id="Principal">
        <div data-role="header">
            <p> mi primera aplicación movil</p>
            
        </div>
         

    
    <div data-role="contenido">
        
        <p> contenido de la aplicación movil</p>
    </div>
    <div data-role="contenido">
        
        <a href="#articulo" data-role="button" data-transition="slideup">Abrir pagina con slideup</a>
         <a href="#articulo" data-role="button" data-transition="slidedown">Abrir pagina con slidedown</a>
          <a href="#articulo" data-role="button" data-transition="flip">Abrir pagina con flip</a>
          <a href="#articulo" data-role="button" data-transition="pop">Abrir pagina con pop</a>
    </div>
        </div>
     <div data-role="page" id="articulo">
        <div data-role="header">
            <a href="#Principal" data-role="button" data-transition="flip">Regresar</a><p> articulo</p>
            
        </div>
         
    
    <div data-role="contenido">
        
        <p> contenido articulo</p>
        <img src="images/800px-ibm_pc_5150.jpg" />
        
        <label for="num1">Numero 1:</label>
        <input type="text" id="num1" placeholder="Numero 1">
          <label for="num1">Numero 1:</label>
         <input type="text" id="num2" placeholder="Numero 2">
         <input type="text" id="resultado" placeholder="resultado">
         <input type="button" value="Sumar" id="btnSuma">
         <input type="button" value="Resta" id="btnResta">
         <input type="button" value="Dividir" id="btnDiv">
         <input type="button" value="Multiplicar" id="btnMult">
    </div>
    <div data-role="contenido">
        <p> pie de articulo</p>
    </div>
        </div>
</body>
</html>
