Jak pliki w formacie Markdown są przetwarzane przez Wordfast Pro i Trados Studio 2022 <!-- omit in toc -->
===

<!-- This here is a comment. And I'd like to create a TOC below -->
<!-- Use this: https://www.markdownguide.org/cheat-sheet/ -->
<!-- Things I need to insert:
- HTML tags, like <code></code>
- (funny thing that markdown kinda works here)
-  -->
- [Wprowadzenie](#introduction)
  - [Czym jest CAT?](#what-is-a-cat)
  - [Dlaczego jest to ważne?](#why-is-this-important)
- Składnia Markdown
  - Informacje ogólne
  - Składnia podstawowa
    - Nagłówek
    - Pogrubienie
    - Kursywa
    - Przekreślenie
    - Lista uporządkowana
    - Lista nieuporządkowana
    - [Połączenie składni podstawowej](#combination-of-basic-syntax)
  - [Odniesienia](#links)
    - [Odniesienia do rozdziałów z nagłówkami](#links-to-sections-with-headers)
    - [Odniesienia do plików](#links-to-files)
    - [Odniesienia do plików graficznych](#links-to-images)
    - [Odniesienia do stron www](#links-to-websites)
    - [Odniesienia do materiałów wideo na YouTube](#links-to-youtube)
    - [Składnia dotycząca odniesień](#syntax-for-links)
  - Cytowanie
    - Cytat blokowy
    - Wiersz kodu
    - Blok kodu
  - Składnia rozszerzona
    - Tabele
    - Lista zadań
    - Emoji
    - Wyróżnienie
    - Indeks dolny
    - Indeks górny
    - Przypisy
    - [Ignorowanie formatowania Markdown](#ignoring-markdown-formatting)
    - Pomijane komentarze
  - Podsumowanie
- [HTML i inne znaczniki](#html-and-other-tags)
  - Informacje ogólne
  - Akapit
  - [Kod](#code)
  - Sekcja zwijana
  - Klawisze klawiaturowe
  - Definicja
  - Wyróżnienie
  - Indeks dolny
  - Indeks górny
  - [Połączenie znaczników i składni Markdown](#combination-of-tags-and-markdown-syntax)
  - Podsumowanie
- Wnioski
- Źródła

# Wprowadzenie

<p>I wrote this file to test how two Computer-Aided Translation programs – Wordfast Pro 7 and Trados 2022 – read Markdown files.</p>
## Czym jest CAT?

Oprogramowanie wspomagające tłumaczenie (ang. [Computer-Aided Translation](https://en.wikipedia.org/wiki/Computer-assisted_translation), zwane powszechnie jako CAT) to program, który pomaga tłumaczom tłumaczyć różnego rodzaju pliki, w tym pliki w formacie Markdown – *.md.

Istnieje **wiele** różnych programów typu CAT. Dwa z nich to *Wordfast Pro* i *Trados Studio 2022*.

## Dlaczego jest to ważne?

Pliki Markdown mają nietypowy rodzaj formatowania. Składnia dla __pogrubienia__ może wyglądać na przykład tak: `__bold__`.  
Powstaje pytanie: Czy program CAT będzie wiedzieć, który symbol jest elementem składnik Markdown, a który został użyty jako część tekstu?

By utrudnić sprawę, w pliku testowym znajduje się również kilka znaczników języka HTML, by sprawdzić, jak są one odczytywane w połączeniu ze składnią Markdown.

Wkrótce się o tym przekonamy.

# Składnia Markdown

## Informacje ogólne

Sprawdzimy następującą składnię Markdown:

1. [Składnia podstawowa](#basic-syntax):
   1. Nagłówek
   2. Pogrubienie
   3. Kursywa
   4. Przekreślenie
   5. Lista uporządkowana
   6. Lista nieuporządkowana
2. [Odniesienia](#links):
   1. [Odniesienia do rozdziałów z nagłówkami](#links-to-sections-with-headers)
   2. [Odniesienia do plików](#links-to-files)
   3. [Odniesienia do plików graficznych](#links-to-images)
   4. [Odniesienia do stron www](#links-to-websites)
   5. [Odniesienia do materiałów wideo na YouTube](#links-to-youtube)
3. [Cytowanie](#quotations):
   1. Cytat blokowy
   2. Wiersz kodu
   3. Blok kodu
4. [Składnia rozszerzona](#extended-syntax):
   1. Tabele
   2. Definicja
   3. Lista zadań
   4. Emoji
   5. Wyróżnienie
   6. Indeks dolny
   7. Indeks górny
   8. Przypisy
   9. [Ignorowanie formatowania Markdown](#ignoring-markdown-formatting)
   10. Pomijane komentarze

---

Pozwoli to sprawdzić, które elementy składni Markdown są – lub **nie są** – odczytywane przez dwa programy CAT:

- _Wordfast Pro_
- _Trados Studio 2022_

## Składnia podstawowa

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

Składnia: `~~This text is in strikethrough.~~`.

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

1. *Pozycja z **bardzo ważnym** tekstem*
   - to **jest po prostu ~~*złe*~~**
   - to jest również __bardzo _ważne___
2. Kolejne _**połączenie** __pogrubienia__ i kursywy_
   1. ~~To jest ***pogrubione**,******, ale głupie*, więc to wykreśliłem~~

Składnia:

```
1. *Item with **very important** text*
   - this **simply ~~*wrong*~~**
   - this is __very _important___ as well
2. Another _**combination** of __bold__ and italic_
   1. ~~this is *__bold__ but folly*, so I crossed it out~~
```

## Odniesienia

Tutaj sprawdzimy, jak różnego rodzaju odniesienia są interpretowane przez *Wordfast Pro* i *Trados Studio 2022*.

### Odniesienia do rozdziałów z nagłówkami

Odniesienie do rozdziału [**Pogrubienie** znajduje się tutaj](#bold).

### Odniesienia do plików

Odniesienie do [pliku Markdown w __repozytorium__ znajduje się _tutaj_](Project-Woźnikowski-2022-11-27.md).

### Odniesienia do plików graficznych

1. Odniesienie do [pliku graficznego w **repozytorium** znajduje się *tutaj*](images/IMG_20200401_210429.jpg).

2. Odniesienie do wyświetlanego pliku graficznego w repozytorium znajduje się tutaj:
   
   ![Rekin](images/IMG_20200401_210429.jpg)

3. Odniesienie do wyświetlanego pliku graficznego w repozytorium z wyświetlanym tekstem podpisu znajduje się tutaj:
   
   ![Rekin](images/IMG_20200401_210429.jpg "Rekin dokumentalista")

4. Odniesienie do wyświetlanego pliku graficznego znajdującego się w internecie:
   
   ![Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e2/2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg/310px-2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg "Cieszyn")

### Odniesienia do stron www

Odniesienie do [mojej strony Translatorion.com znajduje się tutaj](https://translatorion.com/).

### Odniesienia do materiałów wideo na YouTube

Odniesienie do zagnieżdżonego materiału wideo Davida Bowie w serwisie YouTube znajduje się tutaj:

[![](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "Jestem DJ-em,").

### Składnia dotycząca odniesień

Przykład składni: `![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")`

## Cytowanie

Rozdział ten przedstawia różne sposoby cytowania tekstu lub kodu.

### Cytat blokowy

> Oto przykład cytatu.
> 
> Ten cytat ~~nie~~ również obejmuje __podstawową składnię__ i [*odniesienie*](https://en.wikipedia.org/wiki/Link,_West_Virginia "Jestem tym, co gram.").

Składnia:

```
> This is an example of a quote.
> 
> This quote ~~doesn't~~ also includes __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
```

### Wiersz kodu

Oto przykład zdania z wierszem kodem tekstu w `**bold** and _italic_`.

Składnia:

```
`**bold** and _italic_`
```

### Blok kodu

Oto przykład bloku kodu z:

```
1. __Bold__
2. *Italic*
   1. ~~Strikethrough~~
3. > Quotation:
   > - unordered list
4. Link [to a very wise person](https://en.wikipedia.org/wiki/Arthur_Schopenhauer)
```

Składnia: ```` ```code``` ````.

## Składnia rozszerzona

Rozdział ten dotyczy rozszerzonej składni Markdown.

### Tabele

| L.p.| Imię| Nazwisko| Zdjęcie| Wiek|
|:----------|:----------:|:----------:|----------|----------:|
| 1\.| [**Jan _bez Trwogi_**](https://en.wikipedia.org/wiki/John_the_Fearless)| [__Walezjusz__](https://en.wikipedia.org/wiki/House_of_Valois)| ![Jan bez Trwogi](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "Jan bez Trwogi")| 48|
| 2\.| [**Filip *Dobry***](https://en.wikipedia.org/wiki/Philip_the_Good)| [**Walezjusz**](https://en.wikipedia.org/wiki/House_of_Valois)| ![Filip Dobry](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Philip_the_good.jpg/170px-Philip_the_good.jpg "Filip Dobry")| 70|
| 3\.| [__Karol ***Śmiały***__](https://en.wikipedia.org/wiki/Charles_the_Bold)| [__Walezjusz__](https://en.wikipedia.org/wiki/House_of_Valois)| ![Karol Śmiały](https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/Charles_the_Bold_1460.jpg/154px-Charles_the_Bold_1460.jpg "Karol Śmiały")| 44|
| 4\.| [__Maria ***Burgundzka***__](https://en.wikipedia.org/wiki/Mary_of_Burgundy)| [~~Walezjusz~~](https://en.wikipedia.org/wiki/House_of_Valois) [**Habsburg**](https://en.wikipedia.org/wiki/House_of_Habsburg)| ![Maria Burgundzka](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg/169px-Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg "Maria Burgundzka")| 25|

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
- [ ] _**Zadanie** nr trzy_
  - [ ] ___Podzadanie nr trzy-jeden___
  - [ ] ~~Podzadanie nr trzy-dwa~~
- [ ] *__Zadanie nr cztery__*

Składnia: `- [ ] task name`.

### Emoji

Oto przykład listy emoji:

- :wink:
- :uk:
- :cat:
- :tm:
- :aquarius:

Składnia: `:wink:`.

### Wyróżnienie

Oto przykład ==wyróżnienia== w Markdown. ==Nie wszystkie== procesory języka Markdown interpretują ten rodzaj wyróżnienia.

Składnia: `==text==`.

### Indeks dolny

Oto przykład ~indeksu dolnego~ w Markdown. ~Nie wszystkie~ procesory języka Markdown interpretują ten rodzaj indeksu dolnego.

Składnia: `~text~`.

### Indeks górny

Oto przykład ^indeksu górnegot^ w Markdown. ^Nie wszystkie^ procesory języka Markdown interpretują ten rodzaj indeksu górnego.

Składnia: `^text^`.

### Przypisy

Oto przykład zdania z przypisem.\[\^1]

Składnia: `This is a sentence with a footnote.[^1]`.

Oto kolejny przypis. \[\^bignote]

Składnia: `This is another footnote. [^bignote]`.

[\^1]: Informacje dodatkowe

[\^bignote]: Informacje dodatkowe

### Ignorowanie formatowania Markdown

Krótka lista zignorowanego formatowania Markdown:

- \*\*pogrubienie\*\*
- \_kursywa\_
- ~~przekreślenie~~
- \`\*kod\*\`

Składnia: \\\*\\\*pogrubienie**

### Pomijane komentarze

Poniżej tego zdania znajduje się komentarz pomijany przez procesory Markdown:

<!--- Comment --->
Składnia: `<!--- Comment --->`.

## Podsumowanie

**To pod~~~minusowuje~~~^sumowuje^:**

- ___podstawową składnię `Basic`[Markdown](https://en.wikipedia.org/wiki/Markdown):sweat_smile:___

# HTML i inne znaczniki

## Informacje ogólne

Poniżej zostają sprawdzone znaczniki HTML i inne:

1. Akapit
2. [Kod](#code)
3. Sekcja zwijana
4. Klawisze klawiaturowe
5. Definicja
6. Wyróżnienie
7. Indeks dolny
8. Indeks górny
9. [Połączenie znaczników i składni Markdown](#combination-of-tags-and-markdown-syntax)

## Akapit

<p>This is lorem ipsum: lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur ullamcorper ante sit amet aliquet convallis. Integer mollis urna quis velit mattis facilisis.</p>
<p>Vestibulum pulvinar sed eros vitae eleifend. Mauris et ligula metus. Nunc elementum vestibulum arcu quis ultricies. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
Składnia: `<p>Lorem ipsum</p>`.

## Kod

Oto przykład kodu: <code>\*\*pogrubienie\*\* \_kursywa\_</code>

Składnia: `<code>\*\*bold** \_italic_</code>`.

## Sekcja zwijana

Oto zwykła sekcja.

<details><summary>Unroll another section</summary>
<p>
*Tekst* z **różnym** ~~formatowaniem~~.

| L.p.| Imię| Nazwisko|
|----------|----------|----------|
| 1\.| Agnes| **Aardvark**|
| 2\.| Burt| _Butterly_|

Bardzo [ważne odniesienie](https://youtu.be/dQw4w9WgXcQ?t=43).

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

I nigdy nie dotykaj klawisza <kbd>Windows</kbd>!

Składnia: `<kbd>Windows</kbd>`.

## Definicja

Oto przykładowa definicja.

<dl>
"Definition":
<dt> a statement that explains the meaning of a word or phrase </dt>
<dt> a description of the features and limits of something </dt>
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

Składnia: `<mark>text</mark>`.

## Indeks dolny

Oto przykład <sub>indeksu dolnego</sub> HTML. <sub>Nie wszystkie</sub> procesory języka Markdown interpretują ten rodzaj indeksu dolnego.

Składnia: `<sub>text</sub>`.

## Indeks górny

Oto przykład <sup>indeksu dolnego</sup> w HTML. <sup>Nie wszystkie</sup> procesory języka Markdown interpretują ten rodzaj indeksu górnego.

Składnia: `<sup>text</sup>`.

## Połączenie znaczników i składni Markdown

*Oto* __połączenie__ <mark>różnych</mark> <kbd>kluczowych</kbd> <sup>elementów</sup> składni [Markdown](https://en.wikipedia.org/wiki/Markdown) i <code>znaczników</code>.

Składnia:

```
*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <code>tags</code>.
```

## Podsumowanie

Zdaję sobie sprawę, że umieszczenie składni Markdown wewnątrz znaczników HTML, np. `<p>paragraph</p>`, wyłącza je w niektórych procesorach.

# Wnioski

Mam nadzieję, że ta rozległa – ale na pewno nie wyczerpująca – lista znaczników Markdown i HTML będzie stanowić dobrą próbę dla programów *Wordfast Pro* i *Trados Studio 2022*.

Napisałem ten plik Markdown w Visual Studio Code, który nie wyświetla poniższej składni Markdown w oknie podglądu:

- wyróżnienie
- indeks dolny
- indeks górny
- przypisy

Ponadto nie wszystkie znaczniki Markdown lub HTML wyświetlają się w podglądzie Github.

# Źródła

1. [Markdownguide.org](https://www.markdownguide.org/)
2. [Klawisze klawiaturowe](https://meta.stackexchange.com/questions/5527/keyboard-glyphs)
3. [Sekcje zwijane](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections)