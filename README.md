# vue_intro

1) Install extension of google chrome vue.js Devtools and verify the option Allow acces to file URL.

2) Install vue with the link provided in the intro page of vue.org 
```
<script src="https://cdn.jsdelivr.net/npm/vue"></script>

```
3) Create a file and name it main.js

4) First you need to create a Vue instance

```
var app = new Vue ({})
```

5) inside the instance you need to conect the div element that you have created with **el** element and create the data you are going to include to your application and there you need to create your variables.

```
var app = new Vue ({
    el: '#app',
    data: {
        product: 'Socks'
    }
})
```

6) Now our product variable could be use dinamically because vue is **reactive** in our html with an expression {{ variable_example }}}, you could concatenate any kind of data in an expression.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Product App</title>
</head>
<body>
    <div id="app">
        <h1>{{ product + " Medias"}}</h1>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/vue"></script>
    <script src="main.js"></script>
</body>
</html>
```

7) You could perform different acctions inside an expression as:

- Use ternary operator for conditional logic:
```
{{ clicked ? true : false }}
```

- Run methods on your data among other use cases:

```
{{ message.split('').reverse().join('') }}
```

