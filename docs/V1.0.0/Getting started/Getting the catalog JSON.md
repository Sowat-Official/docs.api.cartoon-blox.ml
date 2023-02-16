<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/default.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
<script>hljs.highlightAll();</script>

#Now let's get the catalog items in a JSON format
This will allow you to show the catalog on your site!
```js
//add the object in {} to your import statement
import { init, getCatalogItems } from "https://api.cartoon-blox.ml/staticAPI/@1.0.0/app.js";

//The entire catalog
const catalog = getCatalogItems(config)

//Printing it in the console
console.log(catalog)
```
Result:
<img src='https://drive.google.com/uc?id=16rKmYnlyIytYg5LWhFKOk04GcCv5y11H'>
The result will always be different because if the catalog updates the result updates

The images are hosted on google drive so if something is down the images of the API are not