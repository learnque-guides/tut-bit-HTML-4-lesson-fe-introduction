# iframe

Paprastai tariant `iframe`, tai naršyklė naršyklėje :D

```html
<figure>
  <iframe src="https://www.youtube.com/embed/4Fqg43ozz7A"></iframe>
</figure>
```
*iframe* turi daug problemu susijusiu su resize ir kartais yra sunkumų tinkamai nurodyti plotį.

Šiuo atveju, yra standartiniai būdai kaip tai spręsti:

```css
iframe {
    height: 100%;
    left: 0;
    position: absolute; top: 0;
    width: 100%;
}
```