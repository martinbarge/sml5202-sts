<h1>Example of audio embed, the HTML5 way. No need for Flash.</h1> 
<hr>

<h2>1. The audio player</h2> 

<audio controls> 
<source src="assets/audio/FullExtract.ogg" type="audio/ogg"> 
<source src="assets/audio/FullExtract.mp3" type="audio/mpeg">
Your browser does not support the audio tag.
</audio>


<hr>
<h2>Text that plays sound</h2>
<p>Some text such as <a href="#" onClick="playSound('audio1');event.preventDefault();">psychology</a>.</p>

<hr>
<h2>Buttons that play sounds</h2>

<script> 

function playSound(soundobj) { 
let thissound=document.getElementById(soundobj); 
thissound.play();
}

</script>

<audio id="audio1"> 
<source src="assets/audio/psych.ogg" type="audio/ogg">
<source src="assets/audio/psych.mp3" type="audio/mpeg"> 
</audio> 

<audio id="audio2">
<source src="assets/audio/physiology.ogg" type="audio/ogg">
<source src="assets/audio/physiology.mp3" type="audio/mpeg"> 
</audio> 

<audio id="audio3"> 
<source src="assets/audio/rhino.ogg" type="audio/ogg"> 
<source src="assets/audio/rhino.mp3" type="audio/mpeg"> 
</audio>


<form> 
<input id="submit" type="button" value="psychology" onClick="playSound('audio1')"> 
<input id="submit" type="button" value="physiology" onClick="playSound('audio2')"> 
</form>

<hr>
<h2>An image that plays a sound</h2>
<a id="image" onClick="playSound('audio3')"><img
src="https://upload.wikimedia.org/wikipedia/commons/b/b3/Ostafrikanisches_Spitzmaulnashorn.JPG" style="width:256px; cursor: pointer;" /></a> 
<hr>
