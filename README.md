# Słowa powszechnie używane w klasach CSS

## Obrazy

`image`, `img`, `picture`, `pic` - obrazek

`icon` — ikona

`logo` — logo

`userpic`, `avatar` — userpic, małe zdjęcie użytkownika

`thumbnail`, `thumb` — miniatura

## Tekst

`title`, `subject`, `heading`, `headline`, `caption` — tytuł

`subtitle` — napisy

`slogan` — slogan

`lead`, `tagline` — główny akapit w tekście

`text` - treść tekstowa

`desc` — opis, opcja zawartości tekstu

`excerpt` - fragment tekstu, zwykle używany przed linkiem "Czytaj więcej..."

`quote`, `blockquote` — cytat

`snippet` - przykładowy kod

`link` — link

`copyright`, `copy` - prawa autorskie

## Listy

`list`, `items` - lista, elementy

`item` - element listy

## Bloki

`page` jest elementem głównym strony

`header` - nagłówek (strona lub element)

`footer` - stopka (strony lub elementu)

`section` - sekcja treści (jedna z kilku)

`main`, `body` - główna część (strony lub elementu)

`content` - zawartość elementu

`sidebar` - pasek boczny (strony lub elementu)

`aside` - blok z dodatkowymi informacjami

`widget` - widżet np. na pasku bocznym

## Układ

`wrapper`, `wrap` - opakowanie, zwykle zewnętrzne

`inner` - opakowanie wewnętrzne

`container`, `holder`, `box` — pojemnik

`grid` - układ (strona lub element) w formie siatki (zwykle zawiera `row` i `col`)

`row` - kontener ciągów

`col`, `column` - kontener kolumny

## Sterowanie

`button`, `btn` — przycisk, np. służący do wysłania formularza

`control` - element sterujący, np. strzałki do przodu/do tyłu w galerii zdjęć, przyciski sterowania suwakiem

`dropdown` - lista rozwijana

## wyrażenia multimedialne

`phone`, `mobile` — urządzenia mobilne

`phablet` - telefony z dużymi ekranami (6-7")

`tablet` — tabletki

`notebook`, `laptop` — laptopy

`desktop` - komputery stacjonarne

## Wymiary

`tiny` - mały, malutki

`small`

`medium`

`big`, `large`

`huge` - ogromny

`narrow` - wąski

`wide` - szeroki

## Różnorodny

`search` - szukaj

`socials` — blok ikon mediów społecznościowych

`advertisement`, `adv`, `commercial`, `promo` - blok reklamowy (wycinany przez Adblock, nie zaleca się używania takich klas do bloków z reklamami wewnętrznymi)

`features`, `benefits` - lista głównych cech produktu, usługi

`slider`, `carousel` - slider, element interaktywny z przewijaniem treści

`pagination` - paginacja

`user`, `author` — użytkownik, autor wpisu lub komentarza

`meta` - blok z dodatkowymi informacjami, np. blok tagów i dat w poście

`cart`, `basket` - kosz

`breadcrumbs` - łańcuch nawigacji, "breadcrumbs"

`more`, `all` — link do pełnej informacji

`modal` - okno modalne (dialogowe).

`popup` — wyskakujące okienko

`tooltip`, `tip` — podpowiedzi

`preview` - ogłoszenie, fragment, np. news lub post, może składać się z tytułu, opisu i zdjęcia. Oczekiwany link do pełnej wersji

`overlay` - warstwa nakładki, np. do przyciemniania obrazów lub tworzenia okien modalnych

## Stany

`active`, `current` - aktywny element, np. aktualna pozycja menu

`visible` — widoczny element

`hidden` - element ukryty

`error` — stan błędu

`warning` — stan ostrzeżenia

`success` — status pomyślnego zakończenia zadania

`pending` - stan oczekiwania, np. przed zmianą statusu na błąd lub powodzenie

## Przykłady użycia

### Prosta lista

```html
<ul class="list">
  <li class="list__item">Pierwszy</li>
  <li class="list__item">Drugi</li>
  <li class="list__item">Trzeci</li>
</ul>
```

### Zdjęcie użytkownika (userpic)

```html
<div class="user">
  <img class="user__img" src="userpic.png" alt="Dormidont Pietrowicz" />
  <a class="user__link" href="#">Dormidont Pietrowicz</a>
</div>
```

### Galeria

```html
<div class="gallery">
  <ul class="gallery__list">
    <li class="gallery__item">
      <img class="gallery__img" src="flowers.jpg" alt="Kwiat jak ostatnio" />
    </li>
    <li class="gallery__item">
      <img class="gallery__img" src="trees.jpg" alt="Park Trzech Sosen" />
    </li>
  </ul>
</div>
```

### Nawigacja

```html
<nav class="nav">
  <a class="nav__link nav__link--active">Strona główna</a>
  <a class="nav__link" href="#">Podrzędne</a>
  <a class="nav__link" href="#">Trzeci od końca</a>
  <a class="nav__link" href="#">Przedostatni</a>
  <a class="nav__link" href="#">To koniec</a>
</nav>
```

```html
<nav class="nav">
  <ul class="nav__list">
    <li class="nav__item nav__item--current">
      <a class="nav__link">Strona główna</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Artykuły</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Galeria zdjęć</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Kontakty</a>
    </li>
  </ul>
</nav>
```

### Widżet na pasku bocznym

```html
<div class="widget">
  <h4 class="widget__title">Growna Galaretka</h4>

  <div class="widget__content">
    <p>
      Aby wyhodować towarzyską, przyjazną galaretkę, potrzebujemy rolki gumy
      piankowej, dwóch kilogramów cukru, trzy jajka i pół filiżanki acetonu.
    </p>

    <a class="widget__link" href="#">Nie czytaj dalej...</a>
  </div>
</div>
```

### Blok wiadomości

```html
<div class="news">
  <h3 class="news__title">Wczorajsze wiadomości</h3>

  <ul class="news__list">
    <!-- dodaj klasę bloku do klasy elementu,
             aby utworzyć nową przestrzeń nazw -->
    <li class="news__item item-news">
      <h4 class="item-news__title">Konkurencja płoci w łyżwiarstwie szybkim</h4>
      <div class="item-news__text">
        <p>Zwyciężyła drużyna Kilek z Pietrozawodska</p>

        <a href="#" class="item-news__link">Dowiedz się więcej</a>
      </div>
    </li>

    <li class="news__item item-news">
      <h4 class="item-news__title">
        Naukowcy wyjaśniają rolę pilnika w pielęgnacji paznokci
      </h4>
      <div class="item-news__text">
        <p>
          Brytyjscy naukowcy bardzo docenili ten wkład pilnik w wyrastających
          półtorametrowych paznokciach.
        </p>

        <a href="#" class="item-news__link">Nie czytaj dalej</a>
      </div>
    </li>
  </ul>
</div>
```

### Artykuł lub wpis na blogu (wersja prosta)

```html
<article class="article">
  <h3 class="article__title">Odczuwanie czakr pęczka pietruszki</h3>
  <time class="article__datetime">32 maja, 10:87</time>

  <div class="author-article article__author-article">
    <img
      class="author-article__img"
      src="userpic.png"
      alt="Kleshnya Andreevna"
    />
    <a class="author-article__link" href="#">Kleshnya Andreevna Dolgorukaya</a>
    <div class="author-article__desc">Nasz ekspert od czakr</div>
  </div>

  <div class="article__content">
    Idź na rynek i kup od starszych pań 100-gramowy pęczek pietruszki. Sortuj,
    oczyść z chrząszczy i gąsienic. Pozwól robakom grać wsadź kota, gąsienice do
    garnka z kaktusami, niech jeden będzie Johnem, drugiego Billy'ego, a
    będziesz miał teraz Dziki Zachód w puli. Wróć na pęczek pietruszki. Spójrz
    na niego czule i podrap go odpowiednio za uchem możesz sam lub kot. Wiązanie
    satynową tasiemką koniecznie zawiąż kokardkę. Gratulacje! Teraz masz
    całkowicie udomowiona pęczek pietruszki, która będzie się dobrze bawić,
    goniąc cię na piętach i wykiełkować nasiona w pantoflach.
  </div>
</article>
```

### Artykuł lub wpis na blogu (twardy)

```html
<article class="entry">
  <header class="entry__header">
    <h3 class="entry__title title-entry">
      <a class="title-entry__link" href="#"
        >Gumowe kaczuszki sposobem na samopoznanie</a
      >
    </h3>

    <time class="entry__datetime">32 maja, 10:87</time>
  </header>

  <div class="entry__author author-entry">
    <img
      class="author-entry__img"
      src="userpic.png"
      alt="Vasilisa Sergeyevich"
    />
    <a class="author-entry__link" href="#">Wasilisa Siergiejewicz</a>
  </div>

  <div class="entry__content">
    Zdobądź pudełko pięćdziesięciu gumowych kaczek ze strychu, pozostałe po
    obchodach nowego roku. Z kaczek a płonące świece układają pentagram na
    podłodze pokoju. Usiądź na środku w pozycji lotosu, weź każdą rękę według
    słownika niemiecko-brazylijskiego kaszel, tarcza pełna klatka piersiowa,
    głośno i pewnie, z pełnym zaangażowaniem powiedz „Kwak!”
  </div>

  <div class="entry__tags tags-entry">
    <h4 class="tags-entry__title">Tagi</h4>

    <ul class="tags-entry__list">
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">zrób to sam okrągły taniec</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">pantofle porcelanowe</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">pasta do butów w kuchni</a>
      </li>
    </ul>
  </div>

  <div class="entry__actions actions-entry">
    <ul class="actions-entry__list">
      <li class="actions-entry__item actions-entry__item--read">
        <a class="actions-entry__link" href="#">238 odpowiedzi</a>
      </li>
      <li class="actions-entry__item actions-entry__item--write">
        <a class="actions-entry__link" href="#">Subskrybuj sportloto</a>
      </li>
      <li class="actions-entry__item actions-entry__item--share">
        <a class="actions-entry__link" href="#">Udostępnij</a>
      </li>
    </ul>
  </div>
</article>
```
