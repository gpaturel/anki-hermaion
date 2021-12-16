# Livres

- [ἕρμαιον, Initiation au grec ancien (Ophrys)](http://www.ophrys.fr/fr/catalogue-detail/1676/initiation-au-grec-ancien.html), Jean-Victor VERNHES
- [Manuel d'accentuation grecque (A. Francke)](https://fr1lib.org/book/2838333/b1c820), Charles BALLY

# Dictionnaires

- [dictionnaire grec–français d'Anatole Bailly (éd. Hugo Chávez)](https://bailly.app/)
- [TLG &ndash; Thesaurus Linguae Graecae](http://stephanus.tlg.uci.edu/)
- [Perseus Digital Library](http://www.perseus.tufts.edu/hopper/)
- [Menandri Sententiae (Bibliotheca Augustana)](https://www.hs-augsburg.de/~harsch/graeca/Chronologia/S_ante03/Menandros/men_gn00.html)

# Polices polytoniques / Beta code

- [GFS - Greek Font Society](https://www.greekfontsociety-gfs.gr/)
- [The Best Free Polytonic Greek Fonts](https://www.mrgreekgeek.com/2021/06/03/the-best-free-polytonic-greek-fonts/)
- [WAZU JAPAN's Gallery of Unicode Fonts](http://www.wazu.jp/gallery/Fonts_GreekPoly.html)
- [Ancient Greek Language support for LibreOffice](https://extensions.libreoffice.org/en/extensions/show/ancientgreek)
- [Type polytonic Greek into VS Code](https://marketplace.visualstudio.com/items?itemName=Capatech.betacode)

# Anki Card Templates

<ul>
  <li><a href="#ἕρμαιον-grammaire">grammaire</a></li>
  <li><a href="#ἕρμαιον-vocabulaire">vocabulaire</a></li>
  <li><a href="#ἕρμαιον-déclinaison">déclinaison</a></li>
  <li><a href="#ἕρμαιον-conjugaison">conjugaison</a></li>
  <li><a href="#ἕρμαιον-conjugaison-infinitifs">conjugaison (infinitifs)</a></li>
  <li><a href="#ἕρμαιον-conjugaison-participes">conjugaison (participes)</a></li>
  <li><a href="#ἕρμαιον-version">version</a></li>
</ul>

<section id="ἕρμαιον-grammaire">

# Note Types: ἕρμαιον-grammaire

## Fields

- `Text`

## Cards

### Front Template

```html
{{cloze:Text}}
```

### Back Template

```html
{{cloze:Text}}
```

### Styling

```css
.card {
  font-family: "GFS Didot";
  font-size: 20px;
  text-align: left;
  color: black;
  background-color: white;
  line-height: 1.1;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
.quantité {
  font-size: 90%;
  color: brown;
}
.cloze {
  font-weight: bold;
  color: darkslateblue;
}
.cartouche {
  border: solid;
  border-color: grey;
  border-radius: 3pt;
  border-width: 1px;
  padding-bottom: 1px;
  padding-top: 1px;
}
table {
  width: 100%;
}
td {
  font-weight: normal;
  font-size: 17px;
  text-align: left;
  vertical-align: top;
  padding-right: 10px;
}
td.contraction {
  text-align: center;
}
td.contraction.info {
  opacity: 0.2;
}
td.contraction.opérande {
  background-color: beige;
  font-weight: bold;
}
td.contraction.résultat {
  background-color: thistle;
  font-weight: bold;
}
ul {
  text-align: left;
  padding-left: 15px;
}
li {
  padding-top: 10px;
}
```

</section>
<section id="ἕρμαιον-vocabulaire">

# Note Types: ἕρμαιον-vocabulaire

## Fields

- `grec`
- `français`
- `notes`

## Cards

### Front Template

```html
{{grec}}
```

### Back Template

```html
{{FrontSide}}
<hr/>
<span class="fra">
  {{français}}
  <ul>{{notes}}</ul>
</span>
```

### Styling

```css
:root {
  --désinence: darkred;
  --régime: beige;
  --gr: darkblue;
}
.card {
  font-family: "GFS Didot";
  font-size: 35px;
  text-align: center;
  color: black;
  background-color: white;
  line-height: 1.1;
}
.fra {
  font-size: 22px;
}
.quantité {
  font-size: 50%;
  color: brown;
}
.cas {
  font-variant: small-caps;
  font-size: smaller;
  background-color: var(--régime);
}
.régime {
  background-color: var(--régime);
}
.indo-europ {
  background-color: aliceblue;
}
.contraction {
  font-size: 70%;
}
.désinence {
  font-weight: bold;
  color: var(--désinence);
}
.cartouche {
  border: solid;
  border-color: grey;
  border-radius: 3pt;
  border-width: 1px;
}
table {
  width: 100%;
}
table.décl {
  font-size: 70%;
  color: var(--gr);
}
td {
  font-weight: normal;
  text-align: left;
  vertical-align: top;
  padding-right: 10px;
}
tr.adj {
  background-color: var(--régime);
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
ul {
  font-size: 70%;
  text-align: left;
  padding-left: 15px;
}
li {
  padding-top: 10px;
}
li.propre {
  color: darkgreen;
}
li.propre .fr {
  color: darkgreen;
}
li .gr {
  color: var(--gr);
}
li .fr {
  font-style: italic;
  color: grey;
  font-size: 90%;
}
li.étym {
  color: var(--désinence);
  list-style: square;
}
li.étym .fr {
  color: var(--désinence);
}
li .lat {
  font-style: italic;
}
```

</section>
<section id="ἕρμαιον-déclinaison">

# Note Types: ἕρμαιον-déclinaison

## Fields

- `grec`
- `français`
- `NS (article)`  *(nominatif singulier)*
- `NS`  *(nominatif singulier)*
- `VS`  *(vocatif singulier)*
- `AS (article)`  *(accusatif singulier)*
- `AS`  *(accusatif singulier)*
- `GS (article)`  *(génitif singulier)*
- `GS`  *(génitif singulier)*
- `DS (article)`  *(datif singulier)*
- `DS`  *(datif singulier)*
- `NP (article)`  *(nominatif pluriel)*
- `NP`  *(nominatif pluriel)*
- `VP`  *(vocatif pluriel)*
- `AP (article)`  *(accusatif pluriel)*
- `AP`  *(accusatif pluriel)*
- `GP (article)`  *(génitif pluriel)*
- `GP`  *(génitif pluriel)*
- `DP (article)`  *(datif pluriel)*
- `DP`  *(datif pluriel)*

## Cards

### Front Template

```html
<div style="line-height: .9"><span class="fr">Décliner</span> {{grec}} <span class="fr">({{français}})</span></div>
```

### Back Template

```html
{{FrontSide}}
<hr/>
<table>
  <tr>
    <td class="article">{{NS (article)}}</td>
    <td class="nom">{{NS}}</td>
  </tr>
  <tr>
    <td/>
    <td class="nom">{{VS}}</td>
  </tr>
  <tr>
    <td class="article">{{AS (article)}}</td>
    <td class="nom">{{AS}}</td>
  </tr>
  <tr>
    <td class="article">{{GS (article)}}</td>
    <td class="nom">{{GS}}</td>
  </tr>
  <tr>
    <td class="article">{{DS (article)}}</td>
    <td class="nom">{{DS}}</td>
  </tr>
</table>
<hr/>
<table>
  <tr>
    <td class="article">{{NP (article)}}</td>
    <td class="nom">{{NP}}</td>
  </tr>
  <tr>
    <td/>
    <td class="nom">{{VP}}</td>
  </tr>
  <tr>
    <td class="article">{{AP (article)}}</td>
    <td class="nom">{{AP}}</td>
  </tr>
  <tr>
    <td class="article">{{GP (article)}}</td>
    <td class="nom">{{GP}}</td>
  </tr>
  <tr>
    <td class="article">{{DP (article)}}</td>
    <td class="nom">{{DP}}</td>
  </tr>
</table>
```

### Styling

```css
.card {
  font-family: "GFS Didot";
  font-size: 32px;
  text-align: center;
  color: black;
  background-color: white;
}
.fr {
  font-size: 17px;
}
.désinence {
  font-weight: bold;
  color: darkred;
}
.note {
  font-size: 15px;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 100%;
}
td.article {
  text-align: right;
  vertical-align: top;
  padding-right: 5px;
  width: 25%;
}
td.nom {
  text-align: left;
  vertical-align: top;
  padding-left: 5px;
}
tr:nth-of-type(even) {
  background-color: beige;
}
```

</section>
<section id="ἕρμαιον-conjugaison">

# Note Types: ἕρμαιον-conjugaison

## Fields

- `verbe à conjuguer`
- `traduction`
- `thème - mode`
- `voix`
- `1S`  *(1ère personne du singulier)*
- `1S (note)`  *(1ère personne du singulier)*
- `2S`  *(2ème personne du singulier)*
- `2S (note)`  *(2ème personne du singulier)*
- `3S`  *(3ème personne du singulier)*
- `3S (note)`  *(3ème personne du singulier)*
- `1P`  *(1ère personne du pluriel)*
- `1P (note)`  *(1ère personne du pluriel)*
- `2P`  *(2ème personne du pluriel)*
- `2P (note)`  *(2ème personne du pluriel)*
- `3P`  *(3ème personne du pluriel)*
- `3P (note)`  *(3ème personne du pluriel)*

## Cards

### Front Template

```html
<div style="line-height: .9"><span class="fr">Conjuguer</span> {{1S}}<br>
<span class="fr">({{traduction}})
<p><span class="thème-mode-voix">{{thème - mode}}<br>{{voix}}</span></p>
</span></div>
```

### Back Template

```html
{{FrontSide}}
<hr/>
<table>
  <tr>
    <td class="verbe">{{1S}}</td>
    <td class="note">{{1S (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{2S}}</td>
    <td class="note">{{2S (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{3S}}</td>
    <td class="note">{{3S (note)}}</td>
  </tr>
</table>
<hr/>
<table>
  <tr>
    <td class="verbe">{{1P}}</td>
    <td class="note">{{1P (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{2P}}</td>
    <td class="note">{{2P (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{3P}}</td>
    <td class="note">{{3P (note)}}</td>
  </tr>
</table>
```

### Styling

```css
.card {
  font-family: "GFS Didot";
  font-size: 32px;
  text-align: center;
  color: black;
  background-color: white;
}
.fr {
  font-size: 17px;
}
.thème-mode-voix {
  font-size: 15px;
  font-style: italic;
}
.désinence {
  font-weight: bold;
  color: darkred;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 100%;
}
td.verbe {
  text-align: left;
  vertical-align: bottom;
}
td.note {
  text-align: right;
  vertical-align: bottom;
  font-size: 15px;
}
```

</section>
<section id="ἕρμαιον-conjugaison-infinitifs">

# Note Types: ἕρμαιον-conjugaison-infinitifs

## Fields

- `verbe à conjuguer`
- `traduction`
- `thème - mode`
- `voix`
- `grec`
- `grec (note)`

## Cards

### Front Template

```html
<div style="line-height : .9"><span class="fr">{{traduction}}<br>
<span class="thème-mode-voix">{{thème - mode}}<br>
{{voix}}</span></span></div>
```

### Back Template

```html
{{FrontSide}}
<hr/>
<table>
  <tr>
    <td class="verbe">{{grec}}</td>
    <td class="note">{{grec (note)}}</td>
  </tr>
</table>
```

### Styling

```css
.card {
  font-family: "GFS Didot";
  font-size: 32px;
  text-align: center;
  color: black;
  background-color: white;
}
.fr {
  font-size: 22px;
}
.thème-mode-voix {
  font-size: 15px;
  font-style: italic;
}
.désinence {
  font-weight: bold;
  color: darkred;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 100%;
}
td.verbe {
  text-align: left;
  vertical-align: bottom;
}
td.note {
  text-align: right;
  vertical-align: bottom;
  font-size: 15px;
}
```

</section>
<section id="ἕρμαιον-conjugaison-participes">

# Note Types: ἕρμαιον-conjugaison-participes

## Fields

- `verbe à conjuguer`
- `traduction`
- `thème - mode - genre`
- `voix`
- `NS`  *(nominatif singulier)*
- `NS (note)`  *(nominatif singulier)*
- `VS`  *(vocatif singulier)*
- `VS (note)`  *(vocatif singulier)*
- `AS`  *(accusatif singulier)*
- `AS (note)`  *(accusatif singulier)*
- `GS`  *(génitif singulier)*
- `GS (note)`  *(génitif singulier)*
- `DS`  *(datif singulier)*
- `DS (note)`  *(datif singulier)*
- `NP`  *(nominatif pluriel)*
- `NP (note)`  *(nominatif pluriel)*
- `VP`  *(vocatif pluriel)*
- `VP (note)`  *(vocatif pluriel)*
- `AP`  *(accusatif pluriel)*
- `AP (note)`  *(accusatif pluriel)*
- `GP`  *(génitif pluriel)*
- `GP (note)`  *(génitif pluriel)*
- `DP`  *(datif pluriel)*
- `DP (note)`  *(datif pluriel)*

## Cards

### Front Template

```html
<div style="line-height : .9"><span class="fr">Conjuguer</span> {{NS}}<br>
<span class="fr">({{traduction}})
<p><span class="thème-mode-genre-voix">{{thème - mode - genre}}<br>{{voix}}</span></p>
</span></div>
```

### Back Template

```html
{{FrontSide}}
<hr/>
<table>
  <tr>
    <td class="verbe">{{NS}}</td>
    <td class="note">{{NS (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{VS}}</td>
    <td class="note">{{VS (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{AS}}</td>
    <td class="note">{{AS (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{GS}}</td>
    <td class="note">{{GS (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{DS}}</td>
    <td class="note">{{DS (note)}}</td>
  </tr>
</table>
<hr/>
<table>
  <tr>
    <td class="verbe">{{NP}}</td>
    <td class="note">{{NP (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{VP}}</td>
    <td class="note">{{VP (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{AP}}</td>
    <td class="note">{{AP (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{GP}}</td>
    <td class="note">{{GP (note)}}</td>
  </tr>
  <tr>
    <td class="verbe">{{DP}}</td>
    <td class="note">{{DP (note)}}</td>
  </tr>
</table>
```

### Styling

```css
.card {
  font-family: "GFS Didot";
  font-size: 32px;
  text-align: center;
  color: black;
  background-color: white;
}
.fr {
  font-size: 17px;
}
.thème-mode-genre-voix {
  font-size: 15px;
  font-style: italic;
}
.désinence {
  color: darkred;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 100%;
}
td.verbe {
  text-align: left;
  vertical-align: bottom;
}
td.note {
  text-align: right;
  vertical-align: bottom;
  font-size: 15px;
}
tr:nth-of-type(even) {
  background-color: lavender;
}
```

</section>
<section id="ἕρμαιον-version">

# Note Types: ἕρμαιον-version

## Fields

- `id`
- `grec (brut)`
- `grec (analyse)`
- `français`

## Cards

### Front Template

```html
{{grec (brut)}} <span style="font-size: 40%">[{{id}}]</span>
```

### Back Template

```html
{{FrontSide}}
<hr/>
<span style="font-size: 80%; line-height: 170%">
  {{grec (analyse)}}
</span>
<hr/>
<span class="fr">
  {{français}}
</span>
```

### Styling

```css
:root {
  --cod: darkred;
  --coi: darkslateblue;
  --ccl: darkgreen;
  --cct: darkblue;
  --adv: darkorange;
}
.card {
  font-family: "GFS Didot";
  font-size: 22px;
  text-align: left;
  color: black;
  background-color: white;
  line-height: 1.1;
}
.fr {
  font-size: 80%;
  font-style: italic;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
.bloc, .sujet, .attribut, .prop-infinitive {
  border-left: solid;
  border-right: solid;
  border-color: black;
  border-radius: 3pt;
  border-width: 2px;
  padding-left: 5px;
  padding-right: 5px;
  padding-bottom: 1px;
  padding-top: 1px;
}
.prop-infinitive {
  opacity: 0.6;
  border-color: currentColor;
  border-bottom: solid;
  border-left-width: 3px;
  border-right-width: 3px;
  border-bottom-width: 1px;
}
.sujet, .attribut {
  font-weight: bold;
  border: solid;
  border-width: 2px;
  border-color: grey;
  background-color: beige;
}
.attribut {
  font-weight: normal;
  border-width: 1px;
}
.verbe {
  font-weight: bold;
  border-bottom: solid;
  border-width: 3px;
}
.COD {
  font-style: italic;
  color: var(--cod);
}
.COI {
  font-style: italic;
  color: var(--coi);
}
.CCL {
  font-style: italic;
  color: var(--ccl);
}
.CCT {
  font-style: italic;
  color: var(--cct);
}
.CDN, .adj, .adv {
    font-size: small;
}
.adv {
  color: var(--adv);
}
.COD .adv {
  color: color-mix(in srgb, var(--cod) 50%, var(--adv) 50%);
}
.COI .adv {
  color: color-mix(in srgb, var(--coi) 50%, var(--adv) 50%);
}
.CCL .adv {
  color: color-mix(in srgb, var(--ccl) 50%, var(--adv) 50%);
}
.CCT .adv {
  color: color-mix(in srgb, var(--cct) 50%, var(--adv) 50%);
}
.préposition {
  text-decoration-thickness: 1px;
}
.régime {
  text-decoration: underline wavy;
  text-decoration-thickness: 1px;
}
sub {
  padding-left: 0.4em;
  font-size: 50%;
  color: grey;
}
sup {
  padding-right: 0.4em;
  font-size: 50%;
  opacity: 0.6;
}
```
