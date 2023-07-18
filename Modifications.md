# List of modifications needed for each file to work online

## Phone functionality

### Search this

	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes, minimum-scale=1.0, maximum-scale=5.0">

### Replace with this

	<link rel="stylesheet" href="style.css">

## Icon

	<link rel="icon" sizes="96x96" href="https://andrewme89.github.io/EstariaCampaign/android-chrome-192x192.png">

## NavBar

### In the `<head>` of the file:

	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

#### Search this

	<meta charset="UTF-8">$

#### Replace with this

	<meta charset="UTF-8">\n<style>\n body {\n  margin: 0;\n  font-family: Arial, Helvetica, sans-serif;\n }\n \n .topnav {\n  overflow: hidden;\n  background-color: #333;\n }\n \n .topnav a {\n  float: left;\n  display: none;\n  color: #f2f2f2;\n  text-align: center;\n  padding: 14px 16px;\n  text-decoration: none;\n  font-size: 17px;\n}\n\n.topnav a:hover {\n  background-color: #ddd;\n  color: black;\n}\n\n.topnav a.active {\n  background-color: #863737;\n  color: white;\n}\n\n.topnav .icon {\n  display: none;\n}\n\n@media screen and (max-width: 600px) {\n  .topnav a:not(:first-child) {display: none;}\n  .topnav a.icon {\n    float: right;\n    display: block;\n  }\n}\n\n@media screen and (max-width: 600px) {\n  .topnav.responsive {position: relative;}\n  .topnav.responsive .icon {\n    position: absolute;\n    right: 0;\n    top: 0;\n  }\n  .topnav.responsive a {\n    float: none;\n    display: block;\n    text-align: left;\n  }\n}\n</style>\n

### In the `<body>` of the file:

#### Search this

	<div class="mod-header"></div>

#### Replace with this

	<div class="mod-header">\n	<!-- Top Nav -->\n	<div class="topnav" id="myTopnav">\n	  <a href="https://andrewme89.github.io/EstariaCampaign/" class="active">Back to Dashboard</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html">Session Notes</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/world/world.html">World</a>\n	  <a href="https://andrewme89.github.io/EstariaCampaign/npc-database.html">NPC Database</a>\n	  <a href="javascript:void(0);" class="icon" onclick="myFunction()">\n	    <i class="fa fa-bars"></i>\n	  </a>\n	</div>\n	\n	<!-- Top Nav SCRIPT -->\n	<script>\n	function myFunction() {\n	  var x = document.getElementById("myTopnav");\n	  if (x.className === "topnav") {\n	    x.className += " responsive";\n	  } else {\n	    x.className = "topnav";\n	  }\n	}\n	</script>\n	</div>\n

## Sidebar buttons

### Search this:

`<div class="tree-scroll-area">`(.+)`<div class="tree-item-children">``</div>`
            `</div>`
          `</div>`

### Replace with this:

          <div class="tree-scroll-area">\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/';">Back to Dashboard</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/session-notes/session-notes.html';">Session Notes</button>\n		  <br>\n     		  <br>\n     		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/world/world.html';">World</button>\n		  <br>\n		  <br>\n		  <button onclick="window.location.href = 'https://andrewme89.github.io/EstariaCampaign/npc-database.html';">NPC Database</button>\n		  </div>