script-

<script type='text/javascript'>
//<![CDATA[
<!-- 
document.writeln(" <!DOCTYPE html> "); 
document.writeln(" <html leng=\"es\"> "); 
document.writeln("  "); 
document.writeln(" <style type=\"text/css\"> "); 
document.writeln("  "); 
document.writeln(" 	body "); 
document.writeln(" 	{ "); 
document.writeln(" 		background-color:#fff6f1; "); 
document.writeln(" 		font-family:\"Helvetica\",Arial; "); 
document.writeln(" 	} "); 
document.writeln(" 	#contenido "); 
document.writeln(" 	{ "); 
document.writeln(" 		width:960px; "); 
document.writeln(" 		margin:0 auto; "); 
document.writeln(" 		text-aling:center; "); 
document.writeln(" 	} "); 
document.writeln(" 	h1 "); 
document.writeln(" 	{ "); 
document.writeln(" 		color:#993300; "); 
document.writeln(" 	} "); 
document.writeln(" 	nav ul li "); 
document.writeln(" 	{ "); 
document.writeln(" 		  display:inline-block; "); 
document.writeln(" 		  margin-right:20px; "); 
document.writeln(" 		  color:#1d1d1d; "); 
document.writeln(" 		  cursor: pointer; "); 
document.writeln(" 	} "); 
document.writeln(" 	#text "); 
document.writeln(" 	{ "); 
document.writeln(" 			width:600px; "); 
document.writeln(" 			height:300px; "); 
document.writeln(" 			background-color:#1d1d1d; "); 
document.writeln(" 			color:#fff; "); 
document.writeln(" 			margin:0 auto; "); 
document.writeln(" 			text-align:left; "); 
document.writeln(" 			border-radius:20px; "); 
document.writeln(" 			padding:20px; "); 
document.writeln(" 			box-shadow:0px 0px 20px rgba(0,0,0,2); "); 
document.writeln(" 	} "); 
document.writeln("  "); 
document.writeln(" 	a "); 
document.writeln(" 	{ "); 
document.writeln(" 		color:#99ff33; "); 
document.writeln(" 		font-weight:bold; "); 
document.writeln(" 	} "); 
document.writeln(" 	#canvas "); 
document.writeln(" 	{ "); 
document.writeln(" 		position: absolute; "); 
document.writeln(" 		button:0px; "); 
document.writeln(" 		left:0px; "); 
document.writeln(" 		border:solid;	 "); 
document.writeln(" 	} "); 
document.writeln(" 	meter "); 
document.writeln(" 	{ "); 
document.writeln(" 		width:120px; "); 
document.writeln(" 		margin-left:20px; "); 
document.writeln(" 	} "); 
document.writeln(" 	label "); 
document.writeln(" 	{ "); 
document.writeln(" 		display:block; "); 
document.writeln(" 	} "); 
document.writeln(" <\/style> "); 
document.writeln("  "); 
document.writeln("  "); 
document.writeln("  "); 
document.writeln(" <html lang=\"es\"> "); 
document.writeln(" <head> "); 
document.writeln(" <meta charset='utf-8'> "); 
document.writeln(" <link rel=\"stylesheet\" href= \"jota.css\"> "); 
document.writeln(" <\/head> "); 
document.writeln(" <body> "); 
document.writeln(" 	<div id ='contenido'> "); 
document.writeln(" 	<header> "); 
document.writeln(" 		<hgroup> "); 
document.writeln(" 			<h1>Aplicando las nuevas Etiquetas de HTML5<h1> "); 
document.writeln(" 		<\/hgroup> "); 
document.writeln(" 	<\/header> "); 
document.writeln(" 	<section><div id='textoPr'> "); 
document.writeln(" 		<hgroup> "); 
document.writeln(" 			<center><h1>Media<\/h1> "); 
document.writeln(" 		<\/hgroup> "); 
document.writeln("  "); 
document.writeln(" 		<h1>Video<\/h1><center> "); 
document.writeln(" 			<video id=\"Video1\" width = '350' height= '240' controls 'controls'>  "); 
document.writeln(" 				<source src=\"Introducción a HTML5.mp4\" type=\"video/mp4\" /> "); 
document.writeln("       "); 
document.writeln(" 			<\/video><\/center> "); 
document.writeln("  "); 
document.writeln(" 			<div id=\"buttonbar\"><center> "); 
document.writeln(" 				<button id=\"restart\" onclick=\"restart();\">[]<\/button>  "); 
document.writeln(" 				<button id=\"rew\" onclick=\"skip(-10)\">&lt;&lt;<\/button> "); 
document.writeln(" 				<button id=\"play\" onclick=\"vidplay()\">&gt;<\/button> "); 
document.writeln(" 				<button id=\"fastFwd\" onclick=\"skip(10)\">&gt;&gt;<\/button> "); 
document.writeln(" 			<\/div> <\/center> "); 
document.writeln("  "); 
document.writeln(" 		<h1>Audio<\/h1><center> "); 
document.writeln(" 			<div><audio id=\"audio1\" style=\"width:85%\" controls>Canvas not supported<\/audio> "); 
document.writeln(" 			<\/div> "); 
document.writeln(" 			<div><input type=\"text\" id=\"audioFile\" value=\"11.mp3\" value=\"2.mp3\"size=\"30\" /> "); 
document.writeln(" 			<\/div> "); 
document.writeln(" 				<button id=\"playbutton\" onclick=\"togglePlay();\">&gt;<\/button>   "); 
document.writeln(" 				<button onclick=\"decreaseSpeed();\">&lt;&lt;<\/button> "); 
document.writeln(" 				<button onclick=\"increaseSpeed();\">&gt;&gt;<\/button> "); 
document.writeln(" 				 "); 
document.writeln(" 			<div id=\"rate\"><\/div><\/center> "); 
document.writeln("    "); 
document.writeln(" 	<\/section> "); 
document.writeln(" <\/body> "); 
document.writeln(" <\/html> "); 
document.writeln("  "); 
document.writeln(" <script type=\"text/javascript\">  "); 
document.writeln(" 	var audioElm = document.getElementById(\"audio1\"); "); 
document.writeln("     var ratedisplay = document.getElementById(\"rate\");  "); 
document.writeln("      "); 
document.writeln(" 	audioElm.addEventListener(\"ratechange\", function ()  "); 
document.writeln(" 	{ "); 
document.writeln(" 		ratedisplay.innerHTML = \"Rate: \" + audioElm.playbackRate; "); 
document.writeln("     },  "); 
document.writeln(" 	false); "); 
document.writeln("  "); 
document.writeln("        "); 
document.writeln("        function togglePlay() { "); 
document.writeln("          if (document.getElementById(\"audio1\")) { "); 
document.writeln("  "); 
document.writeln("            if (audioElm.paused == true) { "); 
document.writeln("              playAudio(audioElm);    "); 
document.writeln("            } else { "); 
document.writeln("              pauseAudio(audioElm);  "); 
document.writeln("            } "); 
document.writeln("          } "); 
document.writeln("        } "); 
document.writeln("  "); 
document.writeln("        function playAudio(audioElm) { "); 
document.writeln("          document.getElementById(\"playbutton\").innerHTML = \"Pause\";  "); 
document.writeln("           "); 
document.writeln("          audioElm.src = document.getElementById('audioFile').value; "); 
document.writeln("          audioElm.play(); "); 
document.writeln("        } "); 
document.writeln("  "); 
document.writeln("        function pauseAudio(audioElm) { "); 
document.writeln("          document.getElementById(\"playbutton\").innerHTML = \"play\"; "); 
document.writeln("          audioElm.pause(); "); 
document.writeln("        } "); 
document.writeln("  "); 
document.writeln("         "); 
document.writeln("        function increaseSpeed() { "); 
document.writeln("          audioElm.playbackRate += 1; "); 
document.writeln("        } "); 
document.writeln("  "); 
document.writeln("         "); 
document.writeln("        function decreaseSpeed() { "); 
document.writeln("          if (audioElm.playbackRate <= 1) { "); 
document.writeln("            var temp = audioElm.playbackRate; "); 
document.writeln("            audioElm.playbackRate = (temp / 2);  "); 
document.writeln("          } else { "); 
document.writeln("            audioElm.playbackRate -= 1; "); 
document.writeln("          } "); 
document.writeln("        } "); 
document.writeln("  "); 
document.writeln("      <\/script> "); 
document.writeln(" 	  "); 
document.writeln(" <script type=\"text/javascript\"> "); 
document.writeln("  "); 
document.writeln("     function vidplay() { "); 
document.writeln("        var video = document.getElementById(\"Video1\"); "); 
document.writeln("        var button = document.getElementById(\"play\"); "); 
document.writeln("        if (video.paused) { "); 
document.writeln("           video.play(); "); 
document.writeln("           button.textContent = \"||\"; "); 
document.writeln("        } else { "); 
document.writeln("           video.pause(); "); 
document.writeln("           button.textContent = \">\"; "); 
document.writeln("        } "); 
document.writeln("     } "); 
document.writeln("  "); 
document.writeln("     function restart() { "); 
document.writeln("         var video = document.getElementById(\"Video1\"); "); 
document.writeln("         video.currentTime = 0; "); 
document.writeln("     } "); 
document.writeln("  "); 
document.writeln("     function skip(value) { "); 
document.writeln("         var video = document.getElementById(\"Video1\"); "); 
document.writeln("         video.currentTime += value; "); 
document.writeln("     }       "); 
document.writeln(" <\/script> "); 
document.writeln("  ");
 // -->
//]]>
</script>
=======
