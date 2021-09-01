# input

* Įvesties laukai (`<input>`) yra esminės žiniatinklio formų dalys.
* Įvesties tipas (type) apibrėžiamas kaip atributas ir gali turėti daug reikšmių.
* Pavyzdžiai - text, checkbox, button, color, date, email, password, number,
radio, submit.
radijas.
* Įvestys taip pat gali turėti būtiną atributą (required), tai reiškia, kad negalite
pateikite formą, prieš tai neužpildę informacijos.

---

```html
<form action="/action_page.php" method="POST">
    <input type="text" id="fname" name="fname" required><br><br>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="password" id="password" name="password"><br><br>
    <div>
        <input type="radio" id="huey" name="drone" value="huey" checked>
        <input type="radio" id="dewey" name="drone" value="dewey">
        <input type="radio" id="louie" name="drone" value="louie">
    </div>
    <input type="submit" value="Submit">
</form>
```