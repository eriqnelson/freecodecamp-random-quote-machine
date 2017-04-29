
# Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/FreeCodeCamp/full/ONjoLe/
## Adive: https://deixapaso.wordpress.com/2015/11/03/wrapping-http-content-into-https-via-ajax-request-in-codepen/


1. User Story: I can click a button to show me a new random quote.
`function getQuote(){
$.ajax(
 {type: 'GET',
  dataType: 'json',
  url: 'https://crossorigin.me/http://api.forismatic.com/api/1.0/?method=getQuote&format=json&lang=en',
  cache: 'false',
  success: function(data){
    console.log(data);
  }
});}`




2. User Story: I can press a button to tweet out a quote.
https://dev.twitter.com/web/tweet-button

text =text[0 to 137]+ “…” if text.length>140
