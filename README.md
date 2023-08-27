<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>pagechange</title>
</head>
<body>
    <script>
        function createDevice(){
           
        const mainDiv = document.getElementById('mainContent');
        const allDivs= mainDiv.getElementsByTagName('div')
        const lastDevice = allDivs[allDivs.length-1].innerHTML;
        const lastElement = lastDevice.split("")[lastDevice.split("").length-2]
        console.log(lastElement)
        const newElement = document.createElement('div');
        newElement.innerHTML='device'+ (Number(lastElement)+1) + " "
        newElement.setAttribute('class', 'card')
        mainDiv.appendChild(newElement);
        }
</script>
    <div>
	<header class="mainHeader">
        <nav class="headerNav">
            <div class="navButton">
              <button class="navButton" onclick="createDevice()"> create Device </button>
            </div>
            <div class="navButton">
                <button class="navButton"> delete Device </button>
            </div>
            <div class="navButton">
                <button class="navButton"> update Device </button>
            </div>

        <nav>
</header>	
	<section class="mainSection">
<nav>
<nav>
	</section>
	<main class="mainPage" id="mainContent">
<div class="card">
    dvice 1
</div>
<div class="card">
 device 2
</div>
<div class="card">
device 3
</div>
	</main>
	<footer>

	</footer>
</div>
<style>
    .mainHeader{
            position: fixed;
    width: 100vw;
    height: 10vh;
    border: 1px solid;
    background-color: aqua;
    }
    .mainSection{
        height: 80vh;
    width: 30vw;
    border: 1px solid;
    position: fixed;
    top: 73px;
    }
    .mainPage{
        height: 80vh;
    width: 70vw;
    border: 1px solid;
    position: fixed;
    top: 73px;
    left: 31%;
        display:flex;
    }
    .card{
        border:1px solid;
        height:50px;
        margin:10px;
    }
    .headerNav{
        display:flex;
    }
          
    .navButton{
margin:10px;
background-color: brown;

    }
</style>
</body>
</html>
