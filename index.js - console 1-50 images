'use strict';



function getDogImage(maxResults) {
  fetch(`https://dog.ceo/api/breeds/image/random/${maxResults}`)
    .then(response => response.json())
    .then(responseJson => 
      console.log(responseJson))
    .catch(error => alert('Something went wrong. Try again later.'));
}



function watchForm() {
  $('form').submit(event => {
    event.preventDefault();
    let maxResults = ${'.js-query'}.val();
    getDogImage(maxResults);
  });
}

$(function() {
  console.log('App loaded! Waiting for submit!');
  watchForm();
});
