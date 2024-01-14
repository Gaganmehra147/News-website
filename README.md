# News-website
This is the code for the news website and it is made from the html and css only.
html code :-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <script src = "new.js"></script>
    <div class="banner">
        <div class="navbar">
            <img src="good-news-high-resolution-logo-transparent.png" class="logo">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Politics</a></li>
                <li><a href="#">Tech</a></li>
                <li><a href="#">Current</a></li>
                <li><a href="#">Entertainment</a></li>
                <li><a href="#">About us</a></li>
            </ul>
        </div>
        <div class="content">

            <h1> GET THE LATEST NEWS FAST</h1>
            <P> Design your carrier according to yourself and make your tommorow very beautiful and happy.</P>

        </div>
    </div>

    
</body>
</html>



css code:-
*{
    margin:0;
    padding:0;
    font-family: 'sans-serif';
}


.banner{

    width: 100%;
    height:100vh;
    background-image: linear-gradient(rgba(0,0,0,0.55),rgba(0,0,0,0.55)),url(background.jpg);
    background-size: cover;
    background-position: center;

}

.navbar{
    width: 85%;
    margin:auto;
    padding:15px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.logo{
    width: 150px;
    cursor: pointer;
}
.navbar ul li{
    list-style: none;
    display:inline-block;
    margin: 0 20px;
    position: relative;

}
.navbar ul li a{
    text-decoration: none;
    color: white;
    text-transform: uppercase;

}
.navbar ul li::after{
    content:'';
    height:3px;
    width:0%;
    background:#009688;
    position: absolute;
    left :0;
    bottom:-5px;
    transition: 0.5s;
}
.navbar ul li:hover::after{
    width:100%;
}
.content{
    width: 100%;
    position:absolute;
    top:50px;
    transform: translateY(50%);
    text-align: center;
    color: #fff;
}
.content h1{
    font-size: 50px;
    margin-top:80px;
}
.content p{
    margin: 20px auto;
    font-weight: 100%;
    line-height: 50px;
}
