
<style>
.iframe-container {
  overflow: hidden;
  padding-top: 56.25%;
  position: relative;
}

.iframe-container iframe {
   border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;
}

// Demo styles


.mainContainer {
  background: url('https://benmarshall.me/wp-content/uploads/2018/08/background.gif');
  font-family: 'Lora', serif;
  font-size: 16px;
  line-height: 1.3;
  margin: 1rem 0;
  text-align: center;
}

/***
h1,
p {
  margin-bottom: 2rem;
}

h1 {
  font-family: 'Poppins', sans-serif;
  font-size: 1.7rem;
}

a {
  color: #31c1ef;
  text-decoration: none;
}

***/


.wrapper {
  background-color: #fff;
  border-radius: 1rem;
  margin: 0 auto;
  max-width: 1020px;
  padding: 2rem;
  width: 100%;
}

</style>

<div class="mainContainer">
<div class="wrapper">
<select name="" id="list" onclick="loadFrame()">
    <option value="shooter">Phrases Shooter Game</option>
    <option value="matching">Phrases matching game</option>
  </select>
  <br><br>
  
  <!--<button type="submit" onclick="myFunction()">Choose Game</button>-->
  
  <div class="iframe-container">
    <iframe id="ifrm" src="https://www.cram.com/flashcards/games/jewel/english-spanish-translations-11085554">
  <p>Your browser does not support iframes.</p>
  </iframe>
  </div>
  
   <p style="font-size:90%;">This <a href="https://benmarshall.me/responsive-iframes/">responsive iframe</a> is courtesy of Ben Marshall's demonstration of <a href="https://benmarshall.me/resize-videos-proportionally-intrinsic-ratios/">intrinsic ratio technique</a>.</p>
</div>
</div>

<script>
function loadFrame() {
  let e = document.getElementById("list");
  let url = e.options[e.selectedIndex].value;
  
  
  if (url == "shooter"){
  let gameUrl = "https://www.cram.com/flashcards/games/stellar-speller/english-spanish-translations-11085554";
  document.getElementById("ifrm").src = gameUrl;
  }
  
  if (url == "matching"){
  let gameUrl = "https://www.cram.com/flashcards/games/jewel/english-spanish-translations-11085554";
  document.getElementById("ifrm").src = gameUrl;
  }
  
  //document.getElementById("myFrame").src = url;
}
</script>
