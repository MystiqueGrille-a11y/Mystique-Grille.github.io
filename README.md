# Mystique-Grille.github.io
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mystique Grille - Scanne & Gagne</title>

<style>
body{
    margin:0;
    background:#000;
    color:white;
    font-family:Arial, sans-serif;
    text-align:center;
}

.container{
    padding:40px 20px;
}

.logo{
    color:#ff0000;
    font-size:40px;
    font-weight:bold;
}

h1{
    color:#fff;
}

button{
    background:#e60000;
    color:white;
    border:none;
    padding:15px 30px;
    font-size:20px;
    border-radius:8px;
    cursor:pointer;
}

.result{
    margin-top:30px;
    padding:20px;
    background:#111;
    border:2px solid #e60000;
    border-radius:10px;
    display:none;
}

.reward{
    font-size:32px;
    font-weight:bold;
    color:#ffcc00;
}
</style>
</head>

<body>

<div class="container">

<div class="logo">MYSTIQUE GRILLE</div>

<h1>🎉 SCANNE & GAGNE 🎉</h1>

<p>Clique sur le bouton pour découvrir ta récompense.</p>

<button onclick="revealReward()">
Découvrir mon gain
</button>

<div class="result" id="result">
<h2>Félicitations !</h2>
<div class="reward" id="reward"></div>
</div>

</div>

<script>

function revealReward(){

const rewards = [

"🍕 PIZZA GRATUITE",

"🚚 LIVRAISON GRATUITE",

"💸 RÉDUCTION DE 50%",

"🥤 BOISSON OFFERTE"

];

const randomReward =
rewards[Math.floor(Math.random()*rewards.length)];

document.getElementById("reward").innerHTML = randomReward;

document.getElementById("result").style.display="block";

}

</script>

</body>
</html>
