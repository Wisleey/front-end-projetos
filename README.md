<!DOCTYPE html>
<html lang="en">
<head>
    <title>Botoes animados</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <link rel="stylesheet" href="css/main.css">
</head> 

<body>
    <h1>
        BOTÃO ANIMADO
    </h1>
    <button class="button"><span>Botão 1  </span></button>
    <br>
    <br>
    <br>
   
    <button class="button" id="button1">
        Botão  2   ➔ <i class="fa-solid fa-arrow-right"></i>
    </button>
    <br>
    <br>
    <div class="container">
        <h2><div class="button">
            botão 3
        </h2></div>
</body>
</html>

  
    
=================================================== " CSS '===========================================
    CODIGO CSS
    
    body{
    background-color: rgb(0, 0, 0);


}



button{
    background: #1A73E8;
    cursor: pointer;
    border-radius: 40px;
    width: 400px;
    padding: 20px;
    font-size: 20px;
    text-align: center;
    font-family: sans-serif;


}
button span{
    position: relative;
    transition: 1s;

}

button span:after{
    content: "\22D9";
    position: absolute;
    opacity: 100;
    top: 0%;
    right: -20px;
    transition: 1s;
    width: 20px;


}

button:hover span{
padding-right: 20px;

}

#------------------------------------------


body{
    background-color: rgb(255, 255, 255);
}

#button1{
    font-size: 18px;
    display: flex;
    align-items: center;
    color: rgb(255, 255, 255);
    background: none;
    border: none;
    padding: 14px 22px;
    position: relative;
}

#button1::before{
    content: '';
    position: absolute;
    top: 50%;
    transform: translateY(-50%) translateX(calc(100% + 110px));
    width: 60px;
    height: 60px;
    background: #1A73E8;
    border-radius: 50px;
    transition: transform .25s .25s cubic-bezier(0, 0, .5, 2), width .25s cubic-bezier(0, 0, .5, 2);
    z-index: -1;
}

#button1:hover::before {
    width: 100%;
    transform: translateY(-50%) translateX(-18px);
    transition: transform .25s cubic-bezier(0, 0, .5, 2), width .25s .25s cubic-bezier(0, 0, .5, 2);
}



#button1 i {
    margin-left: 14px;
    transition: transform .25s .4s cubic-bezier(0, 0, .5, 2);
}

#------------------------------------------
h2

    {
    margin: 0;
    padding: 0;
    background-color: rgb(248, 248, 248);
    }

.container
{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.button
{
    position: relative;
    color: cyan;
    letter-spacing: 15px;
    border: 5px solid cyan;
    padding: 50px;
    font-size: 25px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: bold;
    transition: 1.5s;
    border-radius:100px;
}
.button:hover
{
    box-shadow: 0 5px 50px 0 cyan inset,0 5px 50px 0 cyan,
    0 5px 50px 0 cyan inset,0 5px 50px 0 cyan;
    text-shadow: 0 0 5px cyan;
}
   
