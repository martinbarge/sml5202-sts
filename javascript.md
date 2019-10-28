<h1>Introduction to JavaScript</h1>
<h2>Part 1</h2>
<p>this example demonstrates a simple random(ish) sentence generator, using subject + verb + adverb patterns.</p>
<p>Follow the tutorial on QMplus to make one yourself.</p>

<button onclick="makeSentence()">Click me</button>

<p id="demo"></p>

<script>
function makeSentence() {

var person = {
    names: [ "Brian", "Betty", "Fiona", "Freddy", "Mini", "Marvin", "Alice", "Bob", "Jane", "Arthur", "Vincent", "Amy", "He", "She" ],
    verbs: [ "speaks", "eats", "runs", "walks", "drinks" ],
    adverbs: ["slowly", "quickly", "nicely", "noisily", "a lot", "a little", "rarely" ]
   
};
  
var i;
var text = "";
for (i = 0; i < person.names.length; i++) {

  name = person.names[i];
  verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
  adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)]; 
   
   text += name + " " + verb + " " + adv + "<br>";
   
   document.getElementById("demo").innerHTML = text;
 
 }  

}
</script>
