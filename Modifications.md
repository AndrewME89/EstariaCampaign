# List of modifications needed for each file to work online

## Phone Functionality

### Search this:

	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes, minimum-scale=1.0, maximum-scale=5.0">

### Replace with this:

	<link rel="stylesheet" href="lib/styles/style.css">

## Icon

### Search this:

	<link rel="icon" sizes="96x96" href="https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/favicon-96x96.png">

### Replace with this	:

	<link rel="icon" sizes="96x96" href="https://andrewme89.github.io/EstariaCampaign/estaria-logo.png">

## NavBar

### Search this:

	<meta charset="UTF-8">

### Replace with this:

	<meta charset="UTF-8">\n
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

### Search this:

	<div class="mod-header"></div>
 
### Replace with this:

          <div class="mod-header">
		  <div class="topnav" id="myTopnav">
	  <a href="https://andrewme89.github.io/EstariaCampaign/" class="active">Back to Dashboard</a>
	  <a href="https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html">Session Notes</a>
	  <a href="https://andrewme89.github.io/EstariaCampaign/world/world.html">World</a>
	  <a href="https://andrewme89.github.io/EstariaCampaign/npc-database.html">NPC Database</a>
	  <a href="https://andrewme89.github.io/EstariaCampaign/party-holdings.html">Party Holdings</a>
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

### Search this:

	<div class="tree-scroll-area">(.+)<div class="tree-item-children"></div>
            </div>
          </div>

### Replace with this:

	<div class="tree-scroll-area">\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/';">Back to Dashboard</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html';">Session Notes</button>\n		  <br>\n     		  <br>\n     		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/world/world.html';">World</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/npc-database.html';">NPC Database</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/party-holdings.html';">Party Holdings</button>\n		  </div>
