script-loader
=============

Simple client script loader

## API

### loadScript(url, [name]) : Promise

- `url` - script url to load
- `name` - script global name (loadScript skip script loading if window[name] defined)

## Usage

```js
loadScript('https://path.to/scritp.js', 'script')
  .then(function () {
    script.doWork();
  })
  .catch(function (e) {
    console.error(e);
  })
```