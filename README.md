# Anleitung für eine einfache Slideshow
## Portfolio Kurs

### Anleitung Download und Einrichtung

1. Installiere Visual Code Studio (VSC) https://code.visualstudio.com/
2. Lade dieses Projekt runter, darin sind alle Files enthalten die du brauchst; klicke oben rechts auf den Button **Clone or Download** und dann auf **Download ZIP**
3. Entpacke das heruntergeladene File 
4. Das darin enthaltene .html file könnt ihr nun im browser öffnen und ihr solltet eine funktionierende Slideshow sehen
5. Öffne VSC und klick **File > Open …** > wähle den heruntergeladenen Ordner aus 

> Ganz unten findest du nochmal allgemeine Hinweise.

### Schritt für Schritt zum Code

Wie im Kurs grob erklärt, bauen wir unsere Struktur im HTML File, unser Styling definieren wir im CSS File und die Funktion im JS (Javascript) File.

In diesem Projekte schreiben wir allerdings nur Javascript wie es von unserem »Slideshow-tool« welches wir verwenden vorgegeben ist:
–> https://swiperjs.com/

## HTML Code

Die vorgegeben Struktur im HTML ist, wie folgt. Alle unsere HTMLElemente sind <div> Tags.
Diese bestehen immer aus einem öffnenden <div> und schliessenden </div> Element. Stelle Sie dir als Behälter für Inhalte vor.

> Dazu mehr hier https://www.designerinaction.de/tipps-tricks/web-development/aufbau-html5/

```
<div class="swiper-container">
    <div class="swiper-wrapper">
        <div class="swiper-slide">Slide 1</div>
        <div class="swiper-slide">Slide 2</div>
        <div class="swiper-slide">Slide 3</div>
    </div>
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>
</div>
```

1. Unsere Gesamte Slideshow spielt sich im div it der Klasse "swiper-container" ab
2. Darin befindet sich auf 2. Ebene der "swiper-wrapper", der "swiper-button-prev" und der "swiper-button-next". Der Wrapper enthält alle unsere Slides "swiper-slide", in dem Fall sind das nur drei, die aber beliebig dupliziert werden können. Darin werden wir unsere Bilder verknüpfen. Prev und Next sind die beiden Buttons, die zur nächsten oder vorherigen Slide führen.

Ein typisches HTML Fils sieht so aus mache dir keine Gedanken darum was da lles drin steht, wichtig ist nur dass du weisst wo du deinen Code reinschreibst.
Kurz erklärt; das äusserte Element ist das <html> darin gibt es ein <head></head> darin sind alle informationen enthalten die nicht im browserfenster zu sehen sind; Beispiel Title, dieser wird  im Browser Tab angezeigt und unser CSS File wird darin verlinkt.

```
<link rel="stylesheet" href="https://unpkg.com/swiper/css/swiper.min.css">
<link rel="stylesheet" href="style.css" />
```
Link 1 verweisst auf das css file von swiper direkt auf der website.
Link 2 verweisst auf inser lokales style.css file, dass am selben ort liegt wie unser index.html

Im Body

```
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <link rel="stylesheet" href="https://unpkg.com/swiper/css/swiper.min.css">
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>

        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

## CSS Code

CSS ist sehr einfach zum schreiben. Allerdings können sehr viele Styles festgelegt werden, die man zum Beispiel hier nachschauen kann: https://www.w3schools.com/css/

Das wichtigste ist, dass ihr Klassen an Elemente verteilen könnt im HTML:

HTML: 
```
<div class="my-class"></div>
```
Die ihr dann im CSS stylen könnt. *Wichtig: Eine Klasse muss im css immer mit einem punkt markiert werden.*

CSS
```
.my-class{
    background-color: red;
}
```

## Javascript Code

Grundsätzliche Hilfestellung

In VSC erstellst du ein File in der Menuleiste oben *File > New File* mit Cmd+S(Mac) Ctrl+S(Window) kannst du den Filnamen und die Endung eintippen. So kannst du .html, .css, .js, etc. -files anlegen. 

Veröffentlichung im Web

Um das Projekt zu veröffentlichen ist die einfachste Variante das Projekt mit einem FTP Client *(bsp. Cyperduck bietet sich als freeware an)* auf deinen Server zu laden.

*–> Dazu findest du meistens auch Anleitungen von deinem Serveranbieter*