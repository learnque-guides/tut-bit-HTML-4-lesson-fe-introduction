# Dar daugiau apie paveikslus

Yra dviejų tipų paveikslai:
* Rastriniai vaizdai - apibrėžiami naudojant pikselių tinklelį. Rastrinio vaizdo faile yra informacijos, tiksliai nurodančios, kur kiekvienas pikselis turi būti dedamas ir kokios spalvos jis turėtų būti. Populiarūs žiniatinklio rastro formatai yra „Bitmap“ (.bmp), PNG (.png), JPEG (.jpg) ir GIF (.gif.)
* Vektoriniai vaizdai apibrėžiami naudojant algoritmus - vektorinio vaizdo faile yra formos ir kelio apibrėžimai, kuriuos kompiuteris gali naudoti norėdamas išsiaiškinti, kaip vaizdas turėtų atrodyti, kai jis pateikiamas ekrane. Žiniatinklyje dažniausiai yra naudojamas SVG formatas, kuris leidžia mums sukurti galingą vektorinę grafiką, skirtą naudoti internete.

Pagrindinis skirtumas tarp vektorinių ir rastrinių vaizdų atsiranda tuomet, kai mes bandome keisti paveikslų mastelį:

<p align="center">
  <img src="image/raster-vector-default-size.png">
</p>
<p align="center">
  <img src="image/raster-vector-zoomed.png">
</p>

Be to, vektorinių vaizdų failai yra daug lengvesni (užima mažiau vietos) nei jų rastriniai atitikmenys, nes jiems reikia tik kelių algoritmų, o ne informacijos apie kiekvieną vaizdo tašką atskirai.
