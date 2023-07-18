# List of modifications needed for each file to work online

## Phone Functionality

### Search this

	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes, minimum-scale=1.0, maximum-scale=5.0">

### Replace with this

	<link rel="stylesheet" href="lib/styles/style.css">

## Icon

	<link rel="icon" sizes="96x96" href="https://andrewme89.github.io/EstariaCampaign/estaria-logo.png">

## Sidebar buttons

### Search this:

`<div class="tree-scroll-area">`(.+)`<div class="tree-item-children"></div>`
            `</div>`
          `</div>`

### Replace with this:

          <div class="tree-scroll-area">\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/';">Back to Dashboard</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html';">Session Notes</button>\n		  <br>\n     		  <br>\n     		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/world/world.html';">World</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/npc-database.html';">NPC Database</button>\n		  </div>

## NavBar

### In the `<head>` of the file:

	<link rel="stylesheet" href="lib/styles/font-awesome.min.css">

### In the `<body>` of the file:

#### Search this

	<div class="mod-header"></div>

#### Replace with this

	<div class="mod-header">\n	<!-- Top Nav -->\n	<div class="topnav" id="myTopnav">\n	  <a href="https://andrewme89.github.io/EstariaCampaign/" class="active">Back to Dashboard</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html">Session Notes</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/world/world.html">World</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/npc-database.html">NPC Database</a>\n	  <a href="javascript:void(0);" class="icon" onclick="myFunction()">\n	    <i class="fa fa-bars"></i>\n	  </a>\n	</div>\n	\n	<!-- Top Nav SCRIPT -->\n	<script>\n	function myFunction() {\n	  var x = document.getElementById("myTopnav");\n	  if (x.className === "topnav") {\n	    x.className += " responsive";\n	  } else {\n	    x.className = "topnav";\n	  }\n	}\n	</script>\n	</div>\n

#### After this

	<meta charset="UTF-8">

#### Paste this _**Check how this functions with the updated style.css before proceeding**_

	<!-- Top Nav Style -->
`<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">`
				
	<!-- Top Nav Style -->	
`<style>
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
</style>`
