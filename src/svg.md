# SVG - standartinis žiniatinklio vektorinis fomratas

SVG yra XML pagrindu sukurta kalba vektorinių vaizdų aprašymui. Iš esmės tai yra žymėjimo kalba (ang. markup languae), kaip ir HTML, išskyrus tai, kad turite daug skirtingų elementų, skirtų apibrėžti figūras, kurias norite rodyti savo ektane, ir efektus, kuriuos norite taikyti toms formoms. SVG skirtas grafikai, o ne turiniui pažymėti. SVG turi daug skirtingų elementų geometriniems formoms nusakyti, pvz., `<circle>` ir `<rect>`. Išplėstinės SVG funkcijos apima: <feColorMatrix> (spalvų keitimas naudojant transformacijos matricą), <animate> (animuoti jūsų vektorinės grafikos dalis) ir <mask> (uždėti `mask` ant paveikslo).

---

```html
<svg version="1.1"
     baseProfile="full"
     width="300" height="200"
     xmlns="http://www.w3.org/2000/svg">
  <rect width="100%" height="100%" fill="black" />
  <circle cx="150" cy="100" r="90" fill="blue" />
</svg>
```

---
Aukščiau esamo svg vaizdas pateiktas žemiau:

<p align="center">
    <svg version="1.1"
        baseProfile="full"
        width="300" height="200"
        xmlns="http://www.w3.org/2000/svg">
    <rect width="100%" height="100%" fill="black" />
    <circle cx="150" cy="100" r="90" fill="blue" />
    </svg>
</p>

---

Iš aukščiau pateikto pavyzdžio gali susidaryti įspūdis, kad SVG lengva koduoti/formuoti ranka. Taip, galite rankiniu būdu koduoti paprastą SVG teksto redaktoriuje, tačiau sudėtingam vaizdui tai greitai tampa labai sunku. SVG vaizdams kurti dauguma žmonių naudoja vektorinės grafikos redaktorių, pvz., "Inkscape" arba "Illustrator". Šie paketai leidžia jums sukurti įvairias iliustracijas naudojant įvairius grafikos įrankius ir  sukurti apytiksles nuotraukas (pvz., "Inkscape" "Trace Bitmap" funkciją.)

Be iki šiol aprašytų, SVG turi keletą papildomų privalumų:

* Tekstas vektoriniuose vaizduose lieka prieinamas (tai taip pat naudinga jūsų SEO).
* SVG puikiai tinka formuoti/rašyti scenarijus, nes kiekvienas vaizdo komponentas yra elementas, kurį galima sukurti naudojant CSS arba naudojant "JavaScript".

Taigi kodėl kas nors norėtų naudoti rastrinę grafiką per SVG? Na, SVG turi tam tikrų trūkumų:

* SVG gali labai greitai komplikuotis, o tai reiškia, kad failų dydžiai gali padidėti; sudėtingi SVG taip pat gali sulėtinti tinklalapio užsikrovimo laiką naršyklėje.
* SVG gali būti sunkiau sukurti nei rastrinius vaizdus, atsižvelgiant į tai, kokį vaizdą bandote sukurti.
* SVG nepalaikomas senesnėse naršyklėse, todėl gali būti netinkamas, jei savo svetainėje turite palaikyti senesnes „Internet Explorer“ versijas (SVG pradėta palaikyti nuo IE9.)
* Dėl aukščiau aprašytų priežasčių rastrinė grafika neabejotinai tinka sudėtingesniems vaizdams, pvz., nuotraukoms.

Papraščiausias budas įterpti SVG į jūsų puslapį
---

```html
<img
    src="circle-in-rect.svg"
    alt="some circle in rect"
    height="87"
    width="100" />
```

Tiesioginis SVG įterpimas į HTML
---

SVG galima aprašyti tiesiog jūsų HTML :)

```html
<!DOCTYPE html> 
<html>
    <head>
        <title>Test</title>
    </head>
    <body>
        <div>
            <svg width="300" height="200">
                <rect width="100%" height="100%" fill="green" />
            </svg>
        </div>
    </body>
</html>
```