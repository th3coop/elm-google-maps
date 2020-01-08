### Example

```elm
googleMapView : String -> Html Msg
googleMapView googleMapKey =
    Map.init googleMapKey 400
        |> Map.toHtml
```

> Please, take a look at examples/src/Main.elm

### How to install


```
npm install --save-dev https://github.com/PaackEng/google-map\#3.0
npm install --save-dev @webcomponents/webcomponentsjs
elm install PaackEng/elm-google-maps
```

You have to import both items (the order matters)

- @webcomponents/webcomponentsjs/custom-elements-es5-adapter
- @google-web-components/google-map

### Example using create-elm-app:

Add those lines in `index.js`

```js
import '@webcomponents/webcomponentsjs/custom-elements-es5-adapter';
import '@google-web-components/google-map';
```




### How to run the example

> Disclaimer: You must install [create-elm-app](https://github.com/halfzebra/create-elm-app)

```
cd examples/ && ELM_APP_GOOGLE_MAP_KEY=your_key elm-app start
```