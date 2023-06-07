---
title: Output test file — Wordfast, Extract href link URL value
layout: default
nav_exclude: true
---
Jak pliki w formacie Markdown są przetwarzane przez Wordfast Pro, Trados Studio 2022 i Phrase<!-- omit in toc -->
===

<!-- This here is a comment. And I'd like to create a TOC below -->
<!-- Use this: https://www.markdownguide.org/cheat-sheet/ -->
<!-- Things I need to insert:
- HTML tags, like <code></code>
- (funny thing that markdown kinda works here)
-  -->

- [Wprowadzenie](#wprowadzenie)
  - [Czym jest CAT?](#czym-jest-CAT)
  - [Dlaczego jest to ważne?](#dlaczego-jest-to-ważne)
- [Składnia Markdown](#składnia-markdown)
  - [Informacje ogólne](#informacje-ogólne)
  - [składnia-podstawowa](#składnia-podstawowa)
    - [Nagłówek](#nagłówek)
    - [Pogrubienie](#pogrubienie)
    - [Kursywa](#kursywa)
    - [Przekreślenie](#przekreślenie)
    - [Lista uporządkowana](#lista-uporządkowana)
    - [Lista nieuporządkowana](#lista-nieuporządkowana)
    - [Połączenie składni podstawowej](#połączenie-składni-podstawowej)
  - [Odniesienia](#odniesienia)
    - [Odniesienia do rozdziałów z nagłówkami](#odniesienia-do-rozdziałów-z-nagłówkami)
    - [Odniesienia do plików](#odniesienia-do-plików)
    - [Odniesienia do plików graficznych](#odniesienia-do-plików-graficznych)
    - [Odniesienia do stron www](#odniesienia-do-stron-www)
    - [Odniesienia do materiałów wideo na YouTube](#odniesienia-do-materiałów-wideo-na-youtube)
    - [Odnośniki z tekstem podpisu](#odnośniki-z-tekstem-podpisu)
    - [Składnia dotycząca odniesień](#składnia-dotycząca-odniesień)
  - [Cytowanie](#cytowanie)
    - [Cytat blokowy](#cytat-blokowy)
    - [Wiersz kodu](#wiersz-kodu)
    - [Blok kodu](#blok-kodu)
  - [Składnia rozszerzona](#składnia-rozszerzona)
    - [Tabele](#tabele)
    - [Lista zadań](#lista-zadań)
    - [Emoji](#emoji)
    - [Wyróżnienie](#wyróżnienie)
    - [Indeks dolny](#indeks-dolny)
    - [Indeks górny](#indeks-górny)
    - [Przypisy](#przypisy)
    - [Ignorowanie formatowania Markdown](#ignorowanie-formatowania-markdown)
    - [Pomijane komentarze](#pomijane-komentarze)
  - [Podsumowanie](#podsumowanie)
- [HTML i inne znaczniki](#html-i-inne-znaczniki)
  - [Informacje ogólne](#informacje-ogólne-1)
  - [Akapit](#akapit)
  - [Kod](#kod)
  - [Sekcja zwijana](#sekcja-zwijana)
  - [Klawisze klawiaturowe](#klawisze-klawiaturowe)
  - [Definicja](#definicja)
  - [Wyróżnienie](#wyróżnienie-1)
  - [Indeks dolny](#indeks-dolny-1)
  - [Indeks górny](#indeks-górny-1)
  - [Połączenie znaczników i składni Markdown](#połączenie-znaczników-i-składni-markdown)
  - [Czysta składnia HTML z JavaScript](#czysta-składnia-html-z-javascript)
  - [Podsumowanie](#podsumowanie-1)
- [Wnioski](#wnioski)
- [Źródła](#źródła)

# Wprowadzenie

Plik ten powstał do sprawdzenia, jak trzy programy wspomagające tłumaczenie (ang. *Computer-Aided Translation*; CAT) — Wordfast Pro, Trados Studio 2022 i Phrase — odczytują pliki w formacie Markdown.

## Czym jest CAT?
Oprogramowanie wspomagające tłumaczenie (ang. [Computer-Aided Translation](https://en.wikipedia.org/wiki/Computer-assisted_translation), zwane powszechnie jako CAT) to program, który pomaga tłumaczom tłumaczyć różnego rodzaju pliki, w tym pliki w formacie Markdown – *.md.

Istnieje **wiele** różnych programów typu CAT. Trzy z nich to *Wordfast Pro*, *Trados Studio* i *Phrase*.
## Dlaczego jest to ważne?
Pliki Markdown mają nietypowy rodzaj formatowania. Składnia dla __pogrubienia__ może wyglądać na przykład tak: `__bold__`.
Powstaje pytanie: Czy program CAT będzie wiedzieć, który symbol jest elementem składnik Markdown, a który został użyty jako część tekstu?

By utrudnić sprawę, w pliku testowym znajduje się również kilka znaczników języka HTML, by sprawdzić, jak są one odczytywane w połączeniu ze składnią Markdown.

Wkrótce się o tym przekonamy.

# Składnia Markdown

## Informacje ogólne

Sprawdzimy następującą składnię Markdown:
1. [Składnia podstawowa](#składnia-podstawowa):
   1. [Nagłówek](#nagłówek)
   2. [Pogrubienie](#pogrubienie)
   3. [Kursywa](#kursywa)
   4. [Przekreślenie](#przekreślenie)
   5. [Lista uporządkowana](#lista-uporządkowana)
   6. [Lista nieuporządkowana](#lista-nieuporządkowana)
2. [Odniesienia](#odniesienia):
   1. [Odniesienia do rozdziałów z nagłówkami](#odniesienia-do-rozdziałów-z-nagłówkami)
   2. [Odniesienia do plików](#odniesienia-do-plików)
   3. [Odniesienia do plików graficznych](#odniesienia-do-plików-graficznych)
   4. [Odniesienia do stron www](#odniesienia-do-stron-www)
   5. [Odniesienia do materiałów wideo na YouTube](#odniesienia-do-materiałów-wideo-na-youtube)
3. [Cytowanie](#cytowanie):
   1. [Cytat blokowy](#cytat-blokowy)
   2. [Wiersz kodu](#wiersz-kodu)
   3. [Blok kodu](#blok-kodu)
4. [Składnia rozszerzona](#składnia-rozszerzona):
   1. [Tabele](#tabele)
   2. [Definicja](#definicja)
   3. [Lista zadań](#lista-zadań)
   4. [Emoji](#emoji)
   5. [Wyróżnienie](#wyróżnienie)
   6. [Indeks dolny](#indeks-dolny)
   7. [Indeks górny](#indeks-górny)
   8. [Przypisy](#przypisy)
   9. [Ignorowanie formatowania Markdown](#ignorowanie-formatowania-markdown)
   10. [Pomijane komentarze](#pomijane-komentarze)

---

Pozwoli to sprawdzić, które elementy składni Markdown są — lub **nie są** — odczytywane przez trzy programy CAT:
- _Wordfast Pro 8_
- _Trados Studio 2022_
- _Phrase_

## składnia-podstawowa
Rozdział ten dotyczy podstawowej składni Markdown.

### Nagłówek

W tekście użyto trzech rodzajów nagłówków.

Składnia:
```
# Header 1
## Header 2
### Header 3
```

### Pogrubienie

**Ten tekst jest pogrubiony.**
__Ten tekst jest pogrubiony.__

Składnia:
- `**This text is in bold.**`
- `__This text is in bold.__`

### Kursywa

*Ten tekst jest napisany kursywą.*
_Ten tekst jest napisany kursywą._

Składnia:
- `*This text is in italic.*`
- `_This text is in italic._`

### Przekreślenie
~~Ten tekst jest przekreślony.~~

Składnia: `~~This text is in strikethrough.~~`

### Lista uporządkowana
Oto przykład listy uporządkowanej:
1. Pozycja 1
2. Pozycja 2
3. Pozycja 3
   1. Podpozycja 3.1
   2. Podpozycja 3.2

Składnia:
```
1. Item 1
2. Item 2
3. Item 3
   1. Subitem 3.1
   2. Subitem 3.2
```

### Lista nieuporządkowana
Oto przykład listy nieuporządkowanej:
- Pozycja 1
- Pozycja 2
- Pozycja 3
  - Podpozycja 3
  - Podpozycja 3

Składnia:
```
- Item 1
- Item 2
- Item 3
  - Subitem 3
  - Subitem 3
```
### Połączenie składni podstawowej


1. *Punkt z **bardzo ważnym** tekstem*
   - `this **simply ~~*wrong*~~**`
   - to jest również __bardzo _ważne___
2. Kolejne _**połączenie** __pogrubienia__ i kursywy_
   1. `~~this is *__bold__ but folly*, so I crossed it out~~`

Składnia:
```
1. *Item with **very important** text*
   - this **simply ~~*wrong*~~**
   - this is __very _important___ as well
2. Another _**combination** of __bold__ and italic_
   1. ~~this is *__bold__ but folly*, so I crossed it out~~
```

## Odniesienia
Tutaj sprawdzimy, jak różnego rodzaju odniesienia są interpretowane przez *Wordfast Pro*, *Trados Studio 2022* i _Phrase_.

### Odniesienia do rozdziałów z nagłówkami
Odniesienie do rozdziału [**Pogrubienie** znajduje się tutaj](#pogrubienie).

### Odniesienia do plików
Odniesienie do [pliku Markdown w __repozytorium__ znajduje się _tutaj_](README.md).

### Odniesienia do plików graficznych
1. Odniesienie do [pliku graficznego w **repozytorium** znajduje się *tutaj*](images/IMG_20200401_210429.jpg).
2. Odniesienie do wyświetlanego pliku graficznego w repozytorium znajduje się tutaj:
   
   ![Rekin](images/IMG_20200401_210429.jpg)

3. Odniesienie do wyświetlanego pliku graficznego znajdującego się w internecie:
   
   ![Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e2/2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg/310px-2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg "Cieszyn")

### Odniesienia do stron www
Odniesienie do [mojej strony Translatorion.com znajduje się tutaj](https://translatorion.com/).

### Odniesienia do materiałów wideo na YouTube
Odniesienie do zagnieżdżonego materiału wideo Davida Bowie w serwisie YouTube znajduje się tutaj:

[![Jestem DJ-em](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "I am what I play").

### Odnośniki z tekstem podpisu

Poniżej znajduje się kilka przykładów odnośników z tekstem podpisu.

1. Odniesienie do rozdziału [**Pogrubienie** z tekstem podpisu znajduje się tutaj](#pogrubienie "Bolder").
2. Odniesienie do wyświetlanego pliku graficznego w repozytorium z wyświetlanym tekstem podpisu znajduje się tutaj:

![Rekin](images/IMG_20200401_210429.jpg "Rekin dokumentalista")
3. Odniesienie do [mojej strony Translatorion.com znajduje się tutaj](https://translatorion.com/ "I didn't choose translator's life, translator's life chose me").

### Składnia dotycząca odniesień

Składnia dotycząca odniesień — przykłady:
1. `[**Bold** is here](#bold)`
2. `![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")`
3. `[![I am a DJ](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "I am what I play")`

## Cytowanie

Rozdział ten przedstawia różne sposoby cytowania tekstu lub kodu.

### Cytat blokowy

> Oto przykład cytatu.
>
> > Ten cytat znajduje się [wewnątrz cytatu](https://en.wikipedia.org/wiki/A_Dream_Within_a_Dream "Inception before it was cool").
> > >![wewnątrz cytatu](./images/deeper.jpg "Głębokie")
> 
> Ten cytat ~~nie~~ *również* obejmuj*e* __podstawową składnię__ i [*odniesienie*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
> 
> — *Konfuzjusz*
Składnia:
```
> This is an example of a quote.
>
> > This quote is [inside a quote](https://en.wikipedia.org/wiki/A_Dream_Within_a_Dream "Inception before it was cool").
> > >![inside a quote](./images/deeper.jpg "Deep")
> 
> This quote ~~doesn't~~ *also* include*s* __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
> 
> — *Confusius*
```

### Wiersz kodu

Oto przykład zdania z wierszem kodem tekstu w `**bold** and _italic_`.

Składnia:
```
`**bold** and _italic_`
```

### Blok kodu

Oto przykład bloku kodu ze składnią Markdown:
```
1. __Bold__
2. *Italic*
   1. ~~Strikethrough~~
3. > Quotation:
   > - unordered list
4. Link [to a very wise person](https://en.wikipedia.org/wiki/Arthur_Schopenhauer)
```
<!-- TUTAJ DODAĆ JESZCZE CYTAT Z JS-->

Oto przykład bloku kodu ze składnią JavaScript:

```js
// This is the code I found somewhere and adapted to another project.
var interval;

function countdown() {
  clearInterval(interval);
  interval = setInterval( function() {
      var timer = $('.js-timeout').html();
      timer = timer.split(':');
      var minutes = timer[0];
      var seconds = timer[1];
      seconds -= 1;
      if (minutes < 0) return;
      else if (seconds < 0 && minutes != 0) {
          minutes -= 0;
          seconds = 40;
      }
      else if (seconds < 10 && length.seconds != 2) seconds = '0' + seconds;

      $('.js-timeout').html(minutes + ':' + seconds);

      if (minutes == 0 && seconds == 0) clearInterval(interval);
  }, 1000);
}

$('#js-startTimer').click(function () {
  $('.js-timeout').text("00:40");
  countdown();
});

$('#js-resetTimer').click(function () {
  $('.js-timeout').text("00:40");
  clearInterval(interval);
});
```

Składnia (fragment): ` ```js // This is the code I found somewhere and adapted to another project. var interval;``` `

## Składnia rozszerzona

Rozdział ten dotyczy rozszerzonej składni Markdown.

### Tabele

| Lp. | Imię | Nazwisko | Zdjęcie | Wiek |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**Jan**](https://en.wikipedia.org/wiki/John_the_Fearless) | [__Walezjusz__](https://en.wikipedia.org/wiki/House_of_Valois) | ![Jan bez Trwogi](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "Jan bez Trwogi")|   48 |
| 2. | [**Filip *Dobry***](https://en.wikipedia.org/wiki/Philip_the_Good) | [**Walezjusz**](https://en.wikipedia.org/wiki/House_of_Valois) | ![Filip Dobry](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Philip_the_good.jpg/170px-Philip_the_good.jpg "Filip Dobry") | 70 |
| 3. | [__Karol__](https://en.wikipedia.org/wiki/Charles_the_Bold) | [__Walezjusz__](https://en.wikipedia.org/wiki/House_of_Valois) | ![Karol Śmiały](https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/Charles_the_Bold_1460.jpg/154px-Charles_the_Bold_1460.jpg "Karol Śmiały") | 44 |
| 4. | [__Maria __](https://en.wikipedia.org/wiki/Mary_of_Burgundy) | [](https://en.wikipedia.org/wiki/House_of_Valois) [**Habsburg**](https://en.wikipedia.org/wiki/House_of_Habsburg) | ![Maria Burgundzka](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg/169px-Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg "Maria Burgundzka") | 25 |

Składnia (fragment):
```
| No. | Name | Surname | Photo | Age |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**John _the Fearless_**](https://en.wikipedia.org/wiki/John_the_Fearless) | [__Valois__](https://en.wikipedia.org/wiki/House_of_Valois) | ![John the Fearless](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "John the Fearless")|   48 |
```

### Lista zadań

Oto przykład listy zadań:
- [ ] Zadanie nr **jeden**
- [ ] Zadanie nr *dwa*
- [ ] _**Zadanie nr** trzy_
  - [ ] ___Podzadanie nr trzy-jeden___
  - [ ] ~~Podzadanie nr trzy-dwa~~
- [ ] *__Zadanie nr cztery__*

Składnia: `- [ ] task name`

### Emoji

Oto przykład listy emoji:
- :wink:
- :uk:
- :cat:
- :tm:
- :aquarius:

Składnia: `:wink:`

### Wyróżnienie

Oto przykład ==wyróżnienia== w Markdown. ==Nie wszystkie== procesory języka Markdown interpretują ten rodzaj wyróżnienia.

Składnia: `==text==`.

### Indeks dolny

Oto przykład ~indeksu dolnego~ w Markdown. ~Nie wszystkie~ procesory języka Markdown interpretują ten rodzaj indeksu dolnego.

Składnia: `~text~`.

### Indeks górny

Oto przykład ^indeksu dolnego^ w Markdown. ^Nie wszystkie^ procesory języka Markdown interpretują ten rodzaj indeksu górnego.

Składnia: `^text^`.

### Przypisy

Oto przykład zdania z przypisem.[^1]

Składnia: `This is a sentence with a footnote.[^1]`

To jest kolejny przypis [^bignote]

Składnia: `This is another footnote. [^bignote]`

[^1]: Informacje dodatkowe

[^bignote]: Jeszcze więcej informacji dodatkowych

### Ignorowanie formatowania Markdown

Krótka lista zignorowanego formatowania Markdown:
- **pogrubienie**
- _kursywa_
- ~~przekreślenie~~
- `*kod*`

Składnia: \*\*pogrubienie**

### Pomijane komentarze

Poniżej tego zdania znajduje się komentarz pomijany przez procesory Markdown:

<!--- Comment --->

Składnia: `<!--- Comment --->`

## Podsumowanie
<!--- TUTAJ DODAĆ JESZCZE BARDZIEJ ROZWINIĘTĄ PRÓBKĘ TEKSTU --->
**To _pod_~~~minusowuje~~~ ^sumowuje^:**
- ___ składnię `Basic`[Markdown](https://en.wikipedia.org/wiki/Markdown "Cool, innit?"):sweat_smile:___
- *I to wszystko jest w pliku *.md*
- To_jest___z dużą__emfazą — to*jest***z dużą**emfazą

# HTML i inne znaczniki
<!-- TUTAJ JESZCZE DAĆ PO PROSTU BLOK KODU HTML GDZIEŚ-->
## Informacje ogólne

Poniżej zostają sprawdzone znaczniki HTML i inne:
1. [Akapit](#akapit)
2. [Kod](#kod)
3. [Sekcja zwijana](#sekcja-zwijana)
4. [Klawisze klawiaturowe](#klawisze-klawiaturowe)
5. [Definicja](#definicja)
6. [Wyróżnienie](#wyróżnienie-1)
7. [Indeks dolny](#indeks-dolny-1)
8. [Indeks górny](#indeks-górny-1)
9. [Połączenie znaczników i składni Markdown](#połączenie-znaczników-i-składni-markdown)
10. [Czysta składnia HTML z JavaScript](#czysta-składnia-html-z-javascript)

## Akapit

<p>**Oto *lorem ipsum***: lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur ullamcorper ante sit amet aliquet convallis. Integer mollis urna quis velit mattis facilisis.</p>
<p>Vestibulum pulvinar sed eros vitae eleifend. Mauris et ligula metus. Nunc elementum vestibulum arcu quis ultricies. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>

Składnia: `<p>Lorem ipsum</p>`

==**Ważne**==: składnia Markdown jest ignorowana w elementach blokowych, takich jak tag `<p></p>` HTML.

## Kod

To jest przykładowy kod:
- <code><p>Kod dostępu: odrzucony</p></code>
- <code>**pogrubienie** _kursywa_</code>

Składnia:
- `<code>\<p>Access code: Denied\</p></code>`
- `<code>**bold** _italic_</code>`

==**Ważne**==: składnia Markdown **nie jest** ignorowana w elementach typu **span**, takich jak tag `<code></code>` HTML.

## Sekcja zwijana

Oto zwykła sekcja.

<details><summary>Rozwiń kolejną sekcję</summary>
<p>

*Tekst* z __różnym__ ~~formatowaniem~~.

| Nr | Imię | Nazwisko || --- | --- | --- || 1. | Agnes | **Aardvark** || 2. | Burt | _Butterly_ | Bardzo [ważne odniesienie](https://youtu.be/dQw4w9WgXcQ?t=43).

</p>
</details>

Składnia (fragment):
```
<details><summary>Unroll another section</summary>
<p>

*Text* with __different__ ~~formatting~~.

</p>
</details>
```

## Klawisze klawiaturowe

Użyj klawiszy <kbd>W</kbd>, <kbd>S</kbd>, <kbd>A</kbd>, <kbd>D</kbd>, aby poruszyć się postacią w grze komputerowej.

I nigdy nie dotykaj klawisza <kbd>Windows</kbd> :exploding_head:!

Składnia: `<kbd>Windows</kbd>`

## Definicja

Oto przykładowa definicja.
<dl>
„Definicja”:
<dt> twierdzenie, które objaśnia znaczenie słowa lub wyrażenia </dt>
<dt> opis cech i ograniczeń czegoś </dt>
</dl>

Tłumaczenie za [Cambridge Dictionary](https://dictionary.cambridge.org/pl/dictionary/english/definition).

Składnia:
```
<dl>
"Definition":
<dt> a statement that explains the meaning of a word or phrase </dt>
<dt> a description of the features and limits of something </dt>
</dl>
```

## Wyróżnienie

Oto przykład <mark>wyróżnienia</mark> w HTML. <mark>Nie wszystkie</mark> procesory języka Markdown interpretują ten rodzaj wyróżnienia.

Składnia: `<mark>text</mark>`

## Indeks dolny

Oto przykład <sub>indeksu dolnego</sub> HTML. <sub>Nie wszystkie</sub> procesory języka Markdown interpretują ten rodzaj indeksu dolnego.

Składnia: `<sub>text</sub>`

## Indeks górny

Oto przykład <sup>indeksu dolnego</sup> w HTML. <sup>Nie wszystkie</sup> procesory języka Markdown interpretują ten rodzaj indeksu górnego.

Składnia: `<sup>text</sup>`

## Połączenie znaczników i składni Markdown

*Oto* __połączenie__ <mark>różnych</mark> <kbd>kluczowych</kbd> <sup>elementów</sup> składni [Markdown](https://en.wikipedia.org/wiki/Markdown) i <code>znaczników</code> <em>HTML</em>.

Składnia:
```
*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <em>HTML</em> <code>tags</code>.
```
## Czysta składnia HTML z JavaScript

<html>
   <head>
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
      <style>
         .jotaro {
            background-color: #4f8866;
            padding: 30px;
            border: 5px solid #385A6B;
         }
        .wikkeda {
            font-size: 150%;
            font-family: 'Courier New', Courier, monospace;
            color: #385A6B;
            font-style: italic;
        }
    </style>
   </head>
    <body>
      <div class="jotaro">
         <p class="wikkeda">
            Oto przykład tekstu <kbd>HTML</kbd> z dodanymi <a href="https://www.youtube.com/watch?v=F-z6u5hFgPk">stylami</a>.
         </p>
         <p>
            Oto przykład zwykłego tekstu <em>HTML</em> wewnątrz <code>stylu</code> typu *div*.
         </p>
      </div>
      <div>
         <p>
            Oto przykład zwykłego tekstu <em>HTML</em> bez żadnego stylu.
         </p>
         <p>
            Oto przykład skryptu JavaScript, który odlicza z 40 sekund do 0.
         </p>
         <p>   
            Odliczaj: <span class="js-timeout">00:40</span>.
         </p>
            <button id="js-startTimer">Rozpocznij odliczanie</button>
            <button id="js-resetTimer">Zatrzymaj &amp; i zresetuj</button>
            <script src="./timer.js"></script>
      </div>
    </body>
</html>

Składnia:
```html
<html>
   <head>
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
      <style>
         .jotaro {
            background-color: #4f8866;
            padding: 30px;
            border: 5px solid #385A6B;
         }
        .wikkeda {
            font-size: 150%;
            font-family: 'Courier New', Courier, monospace;
            color: #385A6B;
            font-style: italic;
        }
    </style>
   </head>
    <body>
      <div class="jotaro">
         <p class="wikkeda">
            This is an <kbd>HTML</kbd> text with added <a href="https://www.youtube.com/watch?v=F-z6u5hFgPk">styles</a>.
         </p>
         <p>
            This is just a plain <em>HTML</em> text within <code>div</code> style.
         </p>
      </div>
      <div>
         <p>
            This is just a plain <em>HTML</em> text without any style.
         </p>
         <p>
            This is a JavaScript sample that counts down from 40 seconds to 0.
         </p>
         <p>   
            Countdown: <span class="js-timeout">00:40</span>.
         </p>
            <button id="js-startTimer">Start Countdown</button>
            <button id="js-resetTimer">Stop &amp; Reset</button>
            <script src="./timer.js"></script>
      </div>
    </body>
</html>
```

## Podsumowanie

Oto podsumowanie połączenia znaczników `HTML` wewnątrz pliku `*.md`.

# Wnioski

Mam nadzieję, że ta rozległa – ale na pewno nie wyczerpująca – lista znaczników Markdown i HTML będzie stanowić dobrą próbę dla programów *Wordfast Pro*, *Trados Studio 2022* i *Phrase*.

Napisałem ten plik Markdown w Visual Studio Code, który nie wyświetla poniższych elementów w oknie podglądu:
 - wyróżnienie
 - indeks dolny
 - indeks górny
 - przypisy
 - sekcja zwijana
 - definicja
 - JavaScript

Ponadto nie wszystkie znaczniki Markdown lub HTML wyświetlają się w podglądzie Github.

# Źródła

1. [Markdownguide.org](https://www.markdownguide.org/)
2. [Klawisze klawiaturowe](https://meta.stackexchange.com/questions/5527/keyboard-glyphs)
3. [Sekcje zwijane](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections)
4. [Daring Fireball](https://daringfireball.net/projects/markdown/)