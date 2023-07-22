# button-only-css


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    








<a class href="debut_pages_affichable.php"><span>Welcome</span></a>


 
    </script>







</body>
</html>
<style>

*{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body{
        background-color: rgb(5, 5, 5);
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
    }
    
    
    a{
      position: relative;
      background: rgb(22, 21, 21);
      color: white;
      width: 80px;
      height: 80px;
       display: flex;
      align-items: center;
      justify-content: center;
      transition: 0.5s;
      box-shadow: 0 20px 25px blue;
      overflow: hidden;
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-size: 1.2em;
    }
    
    
    a::before{
      content:"";
      position: absolute;
      left: 30px;
      width: 15px;
      height: 15px;
      border-top: 4px solid white;
      border-right: 4px solid white;
      transform: rotate(45deg);
      transition: 0.5s;
    }
    
    
    a::after{
      content:"";
      position: absolute;
      width: 15px;
      height: 15px;
      border-top: 4px solid white;
      border-right: 4px solid white;
      transform: rotate(45deg) translate(-100px, 100px);
      transition: 0.5s;
    }
    
    
    a:hover{
      width: 200px;
      transition-delay: 0.25s;
    }
    
    
    a:hover::before{
      transform: rotate(45deg) translate(150px, -150px);
    }
    
    
    a:hover::after{
      transform: rotate(45deg) translate(-50px, 50px);
      transition-delay: 0.75s;
    }
    
    
    a:hover span{
      visibility: visible;
      transition-delay: 0.5s;
      opacity: 1;
      transform: translate(0px);
    }
    
    
    a span{
      visibility: hidden;
      opacity: 0;
      white-space: nowrap;
      transform: translate(-30px);
      transition: 0.5s;
      margin-left: 35px;
    }
    
    
  
  .typewriter-container {
	display: flex;
	justify-content: flex-start;
	}
  
	.typewriter{
	 position: absolute;
	 top: 33%;
	 left: 35%;
	}
  
  
	.typewriter p {
	  font-family: IBM Plex Mono, monospace;
	font-size: 45px;
	font-weight: lighter;
	overflow: hidden;
	white-space: nowrap;
	position: relative;
	animation: typing 3.5s steps(24);
	color: #ffffffbf;
	}
	.typewriter p::after {
	content: "";
	position: absolute;
	display: block;
	height: 100%;
	width: 1px;
	background: #dadada;
	right: 0;
	top: 0;
	animation: cursor 1s infinite;
	}
	
	@keyframes typing {
	from {width:0}
	to {width: 100%;}
	}
	
	@keyframes cursor {
	0% {
		opacity: 1;
	}
	50% {
		opacity: 0;
	}
	100% {
		opacity: 1;
	}
	}
	
	
	
	
	
	::before, ::after {
	box-sizing: border-box;
	margin: 0;
	padding: 0;
	}


</style>
