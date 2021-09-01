# HTML5 ir media

Naudojami du žymėnis:
* `<audio>` - audio grojimui naudojant įterptinį `player`
* `<video>` - video grojimui naudojant įterptinį `player`

---

```html
<figure>
    <figcaption>Listen to the T-Rex:</figcaption>
    <audio
        controls
        src="/media/cc0-audio/t-rex-roar.mp3">
            Your browser does not support the
            <code>audio</code> element.
    </audio>
</figure>
```

---

```html
<video controls width="250">
    <source src="/media/cc0-videos/flower.webm"
            type="video/webm">

    <source src="/media/cc0-videos/flower.mp4"
            type="video/mp4">

    Sorry, your browser doesn't support embedded videos.
</video>
```

Daugiau informacijos: 
* [Įterptinis audio elementas](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio)
* [Įterptinis video elementas](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)