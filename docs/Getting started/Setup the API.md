#To get started we need to import you JS script in html
That means that you need to make a JS file to use for the API And call it 'app.js'
now in your html we need to do this:
```
<script type='module' src='app.js'></script>
```
that will import your app.js file as a module the module is important it won't work without

now to import the API in your app.js file:
```
import { configuration } from "./config.js";
import { init } from "API//coming soon";

const config = configuration();
const app = init(config);
```
we now also need a config.js file with the configuration:
```
const config = { 
    API_KEY: "", //your API key
    DisplayMessagesFromAPI: "true", // true or false
    DisplayErrorsFromAPI: "true" //true or false
};

export function configuration() {
    return config; //returns the config
};
```
if you wanna know what the config can do read that <a href='../../extra/config'>here</a>