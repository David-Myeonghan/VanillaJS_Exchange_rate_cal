## HTML

- Is there any way to use props to select currencies in select tag in JS?

## JS

- Fetch:

  - is used to make HTTP request to your backend where you're dealing with a database ie., node JS, PHP, or Python
  - can also use third party API, which basically has an end point that we can hit, and we can pass in URL param. Then, it will give us a response, and then we can use that data in our application.
  - 'fetch' is built-in. No need CDN or require.
  - 'GET' doesn't need any parameters or options

  ```
  function calculate() {
  	fetch('items.json').then((res) => console.log(res));
  }
  ```

  This will return Response not JSON data. In fetch, you need to format to what you want.

  ```
  fetch('items.json')
    .then((res) => res.json());
    //.then(data => console.log(data));
    // or,
    //.then((data) => (document.body.innerHTML = data[0].text));
  }
  ```

  If post requrest,

  ```
  fetch('items.json', {
      method: 'POST',
      headers: {
          'Content-Type: application/json'
          ...
        }
      ...
    })
  ```

This returns promise.

As you know, status No.:
200: ok
201: somethings created on server and successful.

300s: redirect

400s: user Error
500s: server Error

- JSON object:
  - is very similar to a JS object.
  - have key-value pairs inside of curly braces, except with JSON, key and any string values will have double-quotes.
  - we can have JSON arrays, arrays of objects by putting bracket'[]'

API: https://www.exchangerate-api.com/
