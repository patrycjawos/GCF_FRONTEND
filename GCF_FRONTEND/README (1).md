---
description: >-
  Czym są i jak działają strony internetowe, jak korzystać z narzędzi
  developerskich (devtools) w przeglądarkach i z edytora kodu (Visual Studio
  Code)
coverY: 0
---

# 1⃣ Wprowadzenie do frontendu

### Strony www&#x20;

Strona internetowa to dokument lub zbiór dokumentów dostępnych w Internecie, które można przeglądać za pomocą przeglądarki internetowej. Każda strona internetowa ma unikalny adres **URL (Uniform Resource Locator)**, który umożliwia jej jednoznaczne zlokalizowanie w sieci.

Strona internetowa może zawierać różne rodzaje treści, takie jak tekst, obrazy, multimedia, formularze, interaktywne elementy, a także skrypty programistyczne. W zależności od celu i funkcji, strony internetowe mogą być statyczne (o treści niezmiennej) lub dynamiczne (o treści, która może się zmieniać w czasie rzeczywistym w odpowiedzi na interakcje użytkownika).

Podział pracy nad stroną internetową często obejmuje dwie główne dziedziny:

1. **Frontend (strona kliencka):** To ta część strony, którą widzi i z której korzysta użytkownik. Frontend odpowiada za prezentację treści, interakcję z użytkownikiem i ogólny wygląd strony. Technologie frontendowe obejmują **HTML (HyperText Markup Language)** do struktury strony, **CSS (Cascading Style Sheets)** do stylizacji i układu, oraz **JavaScript** do programowania interakcji i dynamicznych efektów.

<div data-full-width="true">

<figure><img src=".gitbook/assets/main-qimg-6795e6ef1ca101a38e86eee75ed1189f-lq.jpeg" alt=""><figcaption></figcaption></figure>

</div>

1. **Backend (strona serwerowa):** To ta część strony, która działa po stronie serwera i obsługuje żądania użytkownika oraz zarządza danymi. Backend może korzystać z różnych technologii i języków programowania, takich jak Node.js, Python, Ruby, PHP, czy Java.

Wspólnie, frontend i backend tworzą kompletną strukturę strony internetowej, która umożliwia interakcję użytkowników z treściami i usługami dostępnymi w Internecie.

### Narzędzia developerskie

Testowa strona - [https://www.national-geographic.pl/artykul/jakie-sa-zwierzeta-domowe](https://www.national-geographic.pl/artykul/jakie-sa-zwierzeta-domowe)

<figure><img src=".gitbook/assets/spaces_op3xUUdY3fhD1imRYply_uploads_5hCmQq4mcPt2tkPfW5Qp_Screenshot 2023-11-11 at 15.webp" alt=""><figcaption></figcaption></figure>

**Jak uruchomić devtools?**

* [ ] (prawy przycisk myszy=> zbadaj/inspect)&#x20;
* [ ] **Option + ⌘ + J** (on macOS)
* [ ] Shift + CTRL + J (on Windows/Linux).

### Edytor kodu - Visual Studio Code

**Download:**

{% embed url="https://code.visualstudio.com/download" %}

**Wtyczka przydatne podczas pisania kodu:**

* Prettier – automatyczne formatowanie kodu
* Live Server - automatyczny zapis i odświeżanie kodu w przeglądarce
* Emmet - szybsze pisanie HTML

**Organizacja plików w projekcie**&#x20;

Najprostszą postawową strukturą plików w Visual Studio Code (VSC) podczas pisania strony internetowej może być coś w stylu:

```bash
project-folder/
|-- index.html
|-- styles/
|   |-- style.css
|-- images/
|   |-- image1.jpg
|   |-- image2.png
|-- scripts/
    |-- main.js
```

1. **index.html:** To jest plik główny HTML, który definiuje strukturę twojej strony internetowej.
2. **styles/:** Katalog zawierający pliki CSS. W tym katalogu umieszcza się arkusze stylów, które definiują wygląd strony.
3. **images/:** Katalog dla obrazów używanych na stronie. W tym miejscu przechowujesz pliki graficzne, takie jak jpg, png itp.
4. **scripts/:** Katalog dla plików JavaScript. Tutaj umieszcza się skrypty, które zapewniają interaktywność na stronie.

### Składnia HTML

**Tag HTML** (HyperText Markup Language) jest fundamentalnym elementem w strukturze dokumentu HTML.&#x20;

HTML jest językiem znaczników, co oznacza, że dokumenty HTML składają się z elementów (zwanych tagami), które określają strukturę i znaczenie zawartości dokumentu.

Ogólna struktura tagu HTML wygląda następująco:

```html
<nazwa_tagu atrybut="wartość">Zawartość tagu</nazwa_tagu
```

Przykłady:&#x20;

```html
<h1>To jest nagłówek pierwszego poziomu</h1>

<a href="https://www.przykladowa-strona.com">Przykładowa Strona</a>
```

Przykładowa struktura bazowa strony:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moja Prosta Strona</title>
</head>
<body>

    <header>
        <h1>Witaj na Mojej Stronie!</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#section1">Sekcja 1</a></li>
            <li><a href="#section2">Sekcja 2</a></li>
            <li><a href="#section3">Sekcja 3</a></li>
        </ul>
    </nav>

    <section id="section1">
        <h2>Sekcja 1</h2>
        <p>To jest pierwsza sekcja mojej strony.</p>
    </section>

    <section id="section2">
        <h2>Sekcja 2</h2>
        <p>To jest druga sekcja mojej strony.</p>
        <img src="obraz.jpg" alt="Opis obrazu">
    </section>

    <section id="section3">
        <h2>Sekcja 3</h2>
        <p>To jest trzecia sekcja mojej strony.</p>
        <ul>
            <li>Punkt 1</li>
            <li>Punkt 2</li>
            <li>Punkt 3</li>
        </ul>
    </section>

    <footer>
        <p>&copy; 2023 Moja Strona. Wszelkie prawa zastrzeżone.</p>
    </footer>

</body>
</html>
```



**Lista tagów html - cheatsheet**

{% embed url="https://cheatsheets.shecodes.io/html" %}

{% embed url="https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2012/06/HTML-Cheatsheet-Skillcrush.pdf" %}

{% hint style="info" %}
**Podsumowanie**

* za co odpowiada html, css i js na stronie www?
* do czego służy doctype?



:green\_book:**Materiały dodatkowe:**

[https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction\_to\_HTML/Getting\_started](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction\_to\_HTML/Getting\_started)​
{% endhint %}



