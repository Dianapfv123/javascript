# codigo que señale el caracter que se solicite
<html>
<head>
    <title>Document</title>
</head>
<body>
    <script>
    var espacios=[];
    var nombre=prompt("Teclee su nombre completo: ");
    do {

    var posicion=parseInt(prompt("Teclee la posicion del caracter que desee apuntar: "));

    }while(posicion<0 || posicion>=nombre.length || isNaN(posicion));

    for (var i=0;i<posicion-1;i++) {
    espacios[i]=".";
    }
    document.write(nombre+"<br>");
    document.write(espacios.join(" ")+"^<br>");
    document.write(espacios.join(" ")+posicion);
    </script>
</body>
</html>
