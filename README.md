<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>P&aacute;gina responsive</title>
    <Style>
        * {
            box-sizing: border-box;
        }
        #marco {
            width: 1200px;
            height: 800px;
            display: block;
          
        }
        @media screen and (orientation:portrait){
            #marco{
                width: 600px;
                height: 900px;
                display: block;
            
            }
        }
        #foto {
            width: 100%;
            height: 100%;
            object-fit: cover;


        }
        body{
            background-color: rgb(82, 53, 27);
            display: flex;
            justify-content: center;   }
            

    </Style>
</head>
<body>
    <picture id="marco">
        <source media="(orientation: landscape) and (min-width:1920px)" srcset="Foto1HED.heic" type="image/heic"> 
        <source media="(orientation: landscape) and (min-width:1920px)" srcset="Foto1HED.webp" type="image/webp"> 
        <source media="(orientation: landscape) and (min-width:1920px)" srcset="Foto1HED.jpg" type="image/jpg"> 

        <source media="(orientation: landscape) and (min-width:800px)" srcset="Foto2HED.heic" type="image/heic">
        <source media="(orientation: landscape) and (min-width:800px)" srcset="Foto2HED.webp" type="image/webp">
        <source media="(orientation: landscape) and (min-width:800px)" srcset="Foto2HED.jpg" type="image/jpg">

        <source media="(orientation: portrait) and (min-width:1200px)" srcset="Foto2VED.heic" type="image/heic"> 
        <source media="(orientation: portrait) and (min-width:1200px)" srcset="Foto2VED.webp" type="image/webp"> 
        <source media="(orientation: portrait) and (min-width:1200px)" srcset="Foto2VED.jpg" type="image/jpg"> 

        <source media="(orientation: portrait) and (min-width:600px)" srcset="Foto1VED.heic" type="image/heic"> 
        <source media="(orientation: portrait) and (min-width:600px)" srcset="Foto1VED.webp" type="image/webp"> 
        <source media="(orientation: portrait) and (min-width:600px)" srcset="Foto1VED.jpg" type="image/jpg"> 
        <img id="foto" src="default.jpg">
    </picture>
</div>
</body>
</html>