<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style_3.css">
    
    <div class="container"> 
        <div class="box">
            <div class="cube"></div>
        </div>
    </div>
</head>
<body>
    
</body>
</html>





*{
    margin: 0;
    padding: 0;
    box-sizing: o;
}
 body{
     display: flex;
     justify-content: center;
     align-items: center;
     min-height: 100vh;
     background-color: black;
     overflow: hidden;
 }
 .container {
     position: relative;
     width: 100%;
     transform: rotate(-15deg);
 }
.box {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    -webkit-box-reflect: below 1px linear-gradient(transparent, #0004);
    animation: animateSdvig 1.5s ease-in-out infinite;

}
@keyframes animateSdvig {
    0%{
        transform: translateX(0);
    }
    100%{
        transform: translateX(200px);

    }
    
}
.cube{
    position: relative;
    height: 200px;
    width: 200px;
    background-color: #03e9f4;
    box-shadow: 0 0 0 5px rgba(3, 233, 244, 1),
    0 0  25px rgba(3, 233, 244, 1),
    0 0  50px rgba(3, 233, 244, 1),
    0 0  100px rgba(3, 233, 244, .75),
    0 0  200px rgba(3, 233, 244, .5),
    0 0  300px rgba(3, 233, 244, .25);
    animation: animet 1.5s ease-in-out infinite;
    transform-origin: left bottom;
}
@keyframes animet {
    0%{
        transform:rotate(0deg) ;
    }
    60%{
        transform: rotate(-90deg);
    }
    65%{transform: rotate(-85deg);

    }
    70%{transform: rotate(-90deg);

    }
    75%{transform: rotate(-87.5deg);

    }
    80%, 100%{transform: rotate(-90deg);

    }
}
