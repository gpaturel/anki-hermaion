# Livres
- [ἕρμαιον, Initiation au grec ancien (Ophrys)](http://www.ophrys.fr/fr/catalogue-detail/1676/initiation-au-grec-ancien.html), Jean-Victor VERNHES
- [Manuel d'accentuation grecque (A. Francke)](https://fr1lib.org/book/2838333/b1c820), Charles BALLY

# Dictionnaires
- [dictionnaire grec–français d'Anatole Bailly (éd. Hugo Chávez)](https://bailly.app/)
- [TLG - Thesaurus Linguae Graecae](http://stephanus.tlg.uci.edu/)
- [Perseus Digital Library](http://www.perseus.tufts.edu/hopper/)

# Polices polytoniques / Beta code
- [GFS - Greek Font Society](https://www.greekfontsociety-gfs.gr/)
- [The Best Free Polytonic Greek Fonts](https://www.mrgreekgeek.com/2021/06/03/the-best-free-polytonic-greek-fonts/)
- [WAZU JAPAN's Gallery of Unicode Fonts](http://www.wazu.jp/gallery/Fonts_GreekPoly.html)
- [Ancient Greek Language support for LibreOffice](https://extensions.libreoffice.org/en/extensions/show/ancientgreek)


# Note Types: ἕρμαιον-grammaire

## Fields
- `Text`

## Cards
### Front Template
```
{{cloze:Text}}
```

### Back Template
```
{{cloze:Text}}
```

### Styling
```
.card {
  font-family: "GFS Didot";
  font-size: 20px;
  text-align: center;
  color: black;
  background-color: white;
  line-height: 1.1;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
.cloze {
  font-weight: bold;
  color: blue;
}
td {
  font-weight: normal;
  font-size: 17px;
  text-align: left;
  vertical-align: top;
  padding-right: 10px;
}
li {
  text-align: left;
  margin-left: 0px;
}
```


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
```
<div style="line-height: .9"><span class="fr">Décliner</span> {{grec}} <span class="fr">({{français}})</span></div>
```

### Back Template
```
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
```
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
.desinence {
  font-weight: bold;
  color: blue;
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
  background-color: Lavender;
}
```


# Note Types: ἕρμαιον-vocabulaire

## Fields
- `grec`
- `français`

## Cards
### Front Template
```
{{grec}}
```

### Back Template
```
{{FrontSide}}
<hr/>
<span class="fr">{{français}}</span>
```

### Styling
```
.card {
  font-family: "GFS Didot";
  font-size: 35px;
  text-align: center;
  color: black;
  background-color: white;
  line-height: 1.1;
}
.fr {
  font-size: 22px;
}
.duree {
  font-size: 50%;
  color: brown;
}
.cas {
  font-variant: small-caps;
  background-color: Lavender;
}
.desinence {
  font-weight: bold;
  color: blue;
}
td {
  font-weight: normal;
  text-align: left;
  vertical-align: top;
  padding-right: 10px;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
```


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
```
<div style="line-height: .9"><span class="fr">Conjuguer</span> {{1S}} <span class="fr">({{traduction}})<br>
<span class="theme-mode-voix">{{thème - mode}}<br>
{{voix}}</span></span></div>
```

### Back Template
```
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
```
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
.theme-mode-voix {
  font-size: 15px;
  font-style: italic;
}
.desinence {
  font-weight: bold;
  color: blue;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 115%;
}
td.verbe {
  text-align: left;
  padding-right: 5px;
  vertical-align: middle;
}
td.note {
  text-align: left;
  padding-left: 5px;
  vertical-align: middle;
  font-size: 15px;
}
```


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
```
<div style="line-height : .9"><span class="fr">{{traduction}}<br>
<span class="theme-mode-voix">{{thème - mode}}<br>
{{voix}}</span></span></div>
```

### Back Template
```
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
```
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
.theme-mode-voix {
  font-size: 15px;
  font-style: italic;
}
.desinence {
  font-weight: bold;
  color: blue;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 115%;
}
td.verbe {
  text-align: left;
  padding-right: 5px;
  vertical-align: middle;
}
td.note {
  text-align: left;
  padding-left: 5px;
  vertical-align: middle;
  font-size: 15px;
}
```


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
```
<div style="line-height : .9"><span class="fr">Conjuguer</span> {{NS}} <span class="fr">({{traduction}})<br>
<span class="theme-mode-genre-voix">{{thème - mode - genre}}<br>
{{voix}}</span></span></div>
```

### Back Template
```
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
```
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
.theme-mode-genre-voix {
  font-size: 15px;
  font-style: italic;
}
.desinence {
  font-weight: bold;
  color: blue;
}
@font-face {
  font-family: "GFS Didot";
  src: url('_GFS-Didot.ttf');
}
table {
  width: 115%;
}
td.verbe {
  text-align: left;
  padding-right: 5px;
  vertical-align: middle;
}
td.note {
  text-align: left;
  padding-left: 5px;
  vertical-align: middle;
  font-size: 15px;
}
tr:nth-of-type(even) {
  background-color: Lavender;
}
```
