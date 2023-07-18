# List of modifications needed for each file to work online

## Phone functionality

Remove

	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes, minimum-scale=1.0, maximum-scale=5.0">

Replace with

	<link rel="stylesheet" href="style.css">

## Icon

	<link rel="icon" sizes="96x96" href="https://andrewme89.github.io/EstariaCampaign/android-chrome-192x192.png">

## NavBar

### In the <head> of the file:

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<style>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

.topnav {
  overflow: hidden;
  background-color: #333;
}

.topnav a {
  float: left;
  display: none;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav a:hover {
  background-color: #ddd;
  color: black;
}

.topnav a.active {
  background-color: #863737;
  color: white;
}

.topnav .icon {
  display: none;
}

@media screen and (max-width: 600px) {
  .topnav a:not(:first-child) {display: none;}
  .topnav a.icon {
    float: right;
    display: block;
  }
}

@media screen and (max-width: 600px) {
  .topnav.responsive {position: relative;}
  .topnav.responsive .icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .topnav.responsive a {
    float: none;
    display: block;
    text-align: left;
  }
}
</style>

### In the <body> of the file:

<div class="topnav" id="myTopnav">
  <a href="https://andrewme89.github.io/EstariaCampaign/" class="active">Back to Dashboard</a>
  <a href="https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html">Session Notes</a>
  <a href="https://andrewme89.github.io/EstariaCampaign/world/world.html">World</a>
  <a href="https://andrewme89.github.io/EstariaCampaign/npc-database.html">NPC Database</a>
  <a href="javascript:void(0);" class="icon" onclick="myFunction()">
    <i class="fa fa-bars"></i>
  </a>
</div>

<script>
function myFunction() {
  var x = document.getElementById("myTopnav");
  if (x.className === "topnav") {
    x.className += " responsive";
  } else {
    x.className = "topnav";
  }
}
</script>

## Sidebar buttons

### In this element:

<div class="tree-scroll-area">_____</div>

### Add this
					<button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/';">Back to Dashboard</button>
					<br>
					<br>
					<button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html';">Session Notes</button>
					<br>
					<br>
					<button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/world/world.html';">World</button>
					<br>
					<br>
					<button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/npc-database.html';">NPC Database</button>
