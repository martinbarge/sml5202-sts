<h1>Text from JSON</h1>

<main class="app">

    <section class="quotes">
      <div class="quote-text"></div>
    </section>
    <section class="controls">
     <!-- <a class="tweet button" target="_blank" rel="noopener noreferrer">Tweet</a>-->
      <button type="button" class="new-quote button">New Quote</button>
    </section>

  </main>
  
  <script>
 //const endpoint = 'https://api.whatdoestrumpthink.com/api/v1/quotes/random';
  const endpoint = 'https://api.quotable.io/random';
  //const endpoint = ' http://quotes.rest/';

function getQuote() {
fetch(endpoint)
.then(function (response) {
return response.json();
})
.then(function(data){
//displayQuote(data.message);
displayQuote(`${data.content} —${data.author}`);

console.log(`${data.content} —${data.author}`)
})
.catch(function () {
console.log("Error occurred");
});
}

function displayQuote(quote){
const quoteText = document.querySelector('.quote-text');
quoteText.textContent = quote;

}

const newQuoteButton = document.querySelector('.new-quote');
newQuoteButton.addEventListener('click', getQuote);

  </script>
