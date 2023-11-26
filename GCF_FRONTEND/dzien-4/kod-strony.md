---
coverY: 0
---

# 2 Kod strony

### index.html

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta name="description" content="Moja pierwsza strona internetowa" />

    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Catamaran:wght@100;400;700;900&display=swap"
      rel="stylesheet"
    />

    <link rel="stylesheet" href="styles/normalize.css" />
    <link rel="stylesheet" href="styles/styles.css" />
  </head>
  <body>
    <section id="hero" class="hero-section">
      <div class="container">
        <header class="header">
          <div class="hero-logo">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="60px"
              height="60px"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#bf0034"
            >
              <path
                d="M8 15C12.8747 15 15 12.949 15 8C15 12.949 17.1104 15 22 15C17.1104 15 15 17.1104 15 22C15 17.1104 12.8747 15 8 15Z"
                stroke="#bf0034"
                stroke-width="1.5"
                stroke-linejoin="round"
              ></path>
              <path
                d="M2 6.5C5.13376 6.5 6.5 5.18153 6.5 2C6.5 5.18153 7.85669 6.5 11 6.5C7.85669 6.5 6.5 7.85669 6.5 11C6.5 7.85669 5.13376 6.5 2 6.5Z"
                stroke="#bf0034"
                stroke-width="1.5"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
          <nav>
            <div class="mobile-menu-icon" id="mobile-menu-icon">
              <svg
                class="icon-menu"
                width="24px"
                height="24px"
                stroke-width="1.5"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                color="#fff"
              >
                <path
                  d="M3 5H21"
                  stroke="#fff"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
                <path
                  d="M3 12H21"
                  stroke="#fff"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
                <path
                  d="M3 19H21"
                  stroke="#fff"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
              </svg>

              <svg
                class="icon-close"
                width="24px"
                height="24px"
                stroke-width="1.5"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                color="#fff"
              >
                <path
                  d="M6.75827 17.2426L12.0009 12M17.2435 6.75736L12.0009 12M12.0009 12L6.75827 6.75736M12.0009 12L17.2435 17.2426"
                  stroke="#fff"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
              </svg>
            </div>
            <ul class="menu" id="main-menu">
              <li><a href="#about">O mnie</a></li>
              <li><a href="#interests">Zainteresowania</a></li>
              <li><a href="#photos">Zdjęcia</a></li>
              <li><a href="#contact">Kontakt</a></li>
            </ul>
          </nav>
        </header>

        <div class="hero-content">
          <h1 class="hero-title">Cześć!</h1>
          <p class="hero-lead">
            Mam na imię Ada. Fascynuje mnie astronomia, eksploracja kosmosu, a
            od niedawna też astrofotografia.
          </p>
          <a class="hero-button" href="#about">Poznajmy się</a>
        </div>
      </div>
    </section>

    <section id="about" class="section about-section">
      <div class="container">
        <div class="columns-container columns-2-container">
          <div class="column about-image">
            <img src="images/female-astronaut.jpg" alt="Młoda astronautka" />
          </div>
          <div class="column about-text">
            <h2 class="section-title">O mnie</h2>
            <p><strong>Jestem Ada.</strong></p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nec
              tempus nulla. Vivamus vel lectus sodales, viverra orci sed,
              porttitor metus. Maecenas at metus sed erat malesuada rutrum.
              Quisque ac erat lacinia, tincidunt ligula a, semper nibh.
            </p>
            <p>
              Quisque at erat metus. Vestibulum maximus, risus at luctus
              vestibulum, neque felis tincidunt mauris, quis aliquam ligula ex
              quis neque.
            </p>
            <p>
              Aliquam rutrum, lacus id consequat pharetra, ex ex dignissim
              sapien, et tempor diam mi cursus dui. In a risus posuere,
              efficitur massa malesuada, ultrices est. Nulla risus felis,
              sodales eu ante sed, cursus lacinia orci.
            </p>
            <p>
              Morbi fringilla porta sodales. Integer efficitur vitae mauris in
              maximus. Nam mollis convallis tincidunt. Fusce leo nisl, facilisis
              at sapien ut, egestas efficitur lorem.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="interests" class="section section-violet interests-section">
      <div class="container">
        <div class="columns-container columns-4-container">
          <div class="column">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="100px"
              stroke-width="1.5"
              height="100px"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M18.5 15L5.5 15"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linejoin="round"
              ></path>
              <path
                d="M16 4L8 4"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M9 4.5L9 10.2602C9 10.7376 8.82922 11.1992 8.51851 11.5617L3.48149 17.4383C3.17078 17.8008 3 18.2624 3 18.7398V19C3 20.1046 3.89543 21 5 21L19 21C20.1046 21 21 20.1046 21 19V18.7398C21 18.2624 20.8292 17.8008 20.5185 17.4383L15.4815 11.5617C15.1708 11.1992 15 10.7376 15 10.2602L15 4.5"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M12 9.01L12.01 8.99889"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M11 2.01L11.01 1.99889"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
            <h3 class="interest-name">Odkrycia</h3>
            <p class="interest-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nec
              tempus nulla. Vivamus vel lectus sodales, viverra orci sed,
              porttitor metus. Maecenas at metus sed erat malesuada rutrum.
            </p>
          </div>
          <div class="column">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="100px"
              height="100px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <circle
                cx="12"
                cy="12"
                r="8"
                stroke="#fff"
                stroke-width="1.5"
                stroke-width="1.5"
              ></circle>
              <path
                d="M17.4995 6.34835C19.7975 5.80967 21.4447 5.87208 21.8376 6.66002C22.5686 8.12616 18.6797 11.5491 13.1515 14.3053C7.62327 17.0616 2.5492 18.1074 1.81821 16.6413C1.4263 15.8553 2.36234 14.5067 4.16701 13.0001"
                stroke="#fff"
                stroke-width="1.5"
              ></path>
            </svg>
            <h3 class="interest-name">Kosmos</h3>
            <p class="interest-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nec
              tempus nulla. Vivamus vel lectus sodales, viverra orci sed,
              porttitor metus.
            </p>
          </div>
          <div class="column">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="100px"
              height="100px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M11.4563 2.66509C11.6717 2.2034 12.3283 2.2034 12.5437 2.66509L15.4077 8.80229C15.4673 8.93 15.57 9.03266 15.6977 9.09227L21.8349 11.9563C22.2966 12.1717 22.2966 12.8283 21.8349 13.0437L15.6977 15.9077C15.57 15.9673 15.4673 16.07 15.4077 16.1977L12.5437 22.3349C12.3283 22.7966 11.6717 22.7966 11.4563 22.3349L8.59227 16.1977C8.53266 16.07 8.43 15.9673 8.30229 15.9077L2.16509 13.0437C1.7034 12.8283 1.7034 12.1717 2.16509 11.9563L8.30229 9.09227C8.43 9.03266 8.53266 8.93 8.59227 8.80229L11.4563 2.66509Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
            <h3 class="interest-name">Astronomia</h3>
            <p class="interest-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nec
              tempus nulla. Vivamus vel lectus sodales, viverra orci sed,
              porttitor metus. Maecenas at metus sed erat malesuada rutrum.
              Quisque ac erat lacinia, tincidunt ligula a, semper nibh.
            </p>
          </div>
          <div class="column">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="100px"
              height="100px"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M16.0614 10.4037L14 17L10 17L7.93865 10.4037C7.35085 8.52273 7.72417 6.47307 8.93738 4.92015L11.5272 1.6052C11.7674 1.29772 12.2326 1.29772 12.4728 1.6052L15.0626 4.92015C16.2758 6.47307 16.6491 8.52273 16.0614 10.4037Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M10 20C10 22 12 23 12 23C12 23 14 22 14 20"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M8.5 12.5C5 15 7 19 7 19L10 17"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M15.9312 12.5C19.4312 15 17.4312 19 17.4312 19L14.4312 17"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M12 11C10.8954 11 10 10.1046 10 9C10 7.89543 10.8954 7 12 7C13.1046 7 14 7.89543 14 9C14 10.1046 13.1046 11 12 11Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
            <h3 class="interest-name">Fizyka</h3>
            <p class="interest-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nec
              tempus nulla. Vivamus vel lectus sodales, viverra orci sed,
              porttitor metus.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="photos" class="section photos-section">
      <div class="container">
        <h2 class="photos-title">Zdjęcia</h2>
        <p class="photos-lead">
          To moje ulubione zdjęcia nocnego nieba: Drogi Mlecznej, zorzy polarnej
          i innych pięknych zjawisk, które możemy obserwować na niebie. Od
          niedawna jestem fanką astrofotografii i próbuję swoich sił w robieniu
          nocnych zdjęć.
        </p>
        <div class="columns-container columns-3-container">
          <div class="column">
            <figure>
              <img src="images/startrails-faik-akmd.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Faik Akmd</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
          <div class="column">
            <figure>
              <img src="images/northern-lights-stein-egil-liland.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Stein Egil Liland</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
          <div class="column">
            <figure>
              <img src="images/moon-sevenstorm-juhaszimrus.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Svenstorm Juhaszimrus</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
          <div class="column">
            <figure>
              <img src="images/antenna-igor-mashkov.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Igor Mashkov</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
          <div class="column">
            <figure>
              <img src="images/milky-way-philippe-donn.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Philippe Donn</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
          <div class="column">
            <figure>
              <img src="images/violet-sky-felix-mittermeier.jpg" alt="" />
              <figcaption>
                Zdjęcie autorstwa <strong>Felix Mittermeier</strong> z
                <strong>Pexels</strong>
              </figcaption>
            </figure>
          </div>
        </div>
      </div>
    </section>

    <section id="quote" class="section quote-section section-pink">
      <div class="container">
        <?xml version="1.0" encoding="UTF-8"?><svg
          width="120px"
          height="120px"
          stroke-width="1.5"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          color="#4f247c"
        >
          <path
            d="M10 12H5C4.44772 12 4 11.5523 4 11V7.5C4 6.94772 4.44772 6.5 5 6.5H9C9.55228 6.5 10 6.94772 10 7.5V12ZM10 12C10 14.5 9 16 6 17.5"
            stroke="#4f247c"
            stroke-width="1.5"
            stroke-linecap="round"
          ></path>
          <path
            d="M20 12H15C14.4477 12 14 11.5523 14 11V7.5C14 6.94772 14.4477 6.5 15 6.5H19C19.5523 6.5 20 6.94772 20 7.5V12ZM20 12C20 14.5 19 16 16 17.5"
            stroke="#4f247c"
            stroke-width="1.5"
            stroke-linecap="round"
          ></path>
        </svg>
        <p class="quote-text">
          Nie ma wiedzy bez wyobraźni i&nbsp;nie ma wyobraźni bez wiedzy.
        </p>
        <p class="quote-author">Stanisław Lem, <em>Świat według Lema</em></p>
      </div>
    </section>

    <section id="contact" class="section contact-section">
      <div class="container">
        <h2 class="contact-title">Napisz do mnie</h2>
        <form class="contact-form" name="contactForm">
          <label class="label" for="name">Imię:</label>
          <input
            type="text"
            id="name"
            name="name"
            placeholder="Imię"
            required
          />
          <label class="label" for="email">E-mail:</label>
          <input
            type="email"
            id="email"
            name="email"
            placeholder="imie.nazwisko@mail.com"
            required
          />
          <label class="label" for="message">Miejsce na Twoją wiadomość:</label>
          <textarea id="message" name="message" rows="5" cols="33"> </textarea>
          <button type="submit" class="submit-button" id="form-submit">
            Wyślij
          </button>
        </form>
      </div>
    </section>

    <footer class="footer section-violet">
      <div class="container">
        <div class="copyright">
          <p>&copy; STEAM Academy 2022</p>
          <p>
            Główne zdjęcie autorstwa <strong>Snapwire</strong> z
            <strong>Pexels</strong>
            <br />
            Zdjęcie astronautki autorstwa <strong>Mikhail Nilov</strong> z
            <strong>Pexels</strong>
          </p>
        </div>
        <div class="social">
          <a href="https://instagram.com" target="_blank">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="40px"
              height="40px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M12 16C14.2091 16 16 14.2091 16 12C16 9.79086 14.2091 8 12 8C9.79086 8 8 9.79086 8 12C8 14.2091 9.79086 16 12 16Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M3 16V8C3 5.23858 5.23858 3 8 3H16C18.7614 3 21 5.23858 21 8V16C21 18.7614 18.7614 21 16 21H8C5.23858 21 3 18.7614 3 16Z"
                stroke="#fff"
                stroke-width="1.5"
              ></path>
              <path
                d="M17.5 6.51L17.51 6.49889"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
          <a href="https://facebook.com" target="_blank">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="40px"
              height="40px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M21 8V16C21 18.7614 18.7614 21 16 21H8C5.23858 21 3 18.7614 3 16V8C3 5.23858 5.23858 3 8 3H16C18.7614 3 21 5.23858 21 8Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M11 21C11 18 11 15 11 12C11 9.8125 11.5 8 15 8"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M9 13H11H15"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
          <a href="https://tiktok.com" target="_blank">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="40px"
              height="40px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M21 8V16C21 18.7614 18.7614 21 16 21H8C5.23858 21 3 18.7614 3 16V8C3 5.23858 5.23858 3 8 3H16C18.7614 3 21 5.23858 21 8Z"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M10 12C8.34315 12 7 13.3431 7 15C7 16.6569 8.34315 18 10 18C11.6569 18 13 16.6569 13 15V6C13.3333 7 14.6 9 17 9"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
          <a href="https://youtube.com" target="_blank">
            <?xml version="1.0" encoding="UTF-8"?><svg
              width="40px"
              height="40px"
              stroke-width="1.5"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              color="#fff"
            >
              <path
                d="M14 12L10.5 14V10L14 12Z"
                fill="#fff"
                stroke="#fff"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M2 12.7075V11.2924C2 8.39705 2 6.94939 2.90549 6.01792C3.81099 5.08645 5.23656 5.04613 8.08769 4.96549C9.43873 4.92728 10.8188 4.8999 12 4.8999C13.1812 4.8999 14.5613 4.92728 15.9123 4.96549C18.7634 5.04613 20.189 5.08645 21.0945 6.01792C22 6.94939 22 8.39705 22 11.2924V12.7075C22 15.6028 22 17.0505 21.0945 17.9819C20.189 18.9134 18.7635 18.9537 15.9124 19.0344C14.5613 19.0726 13.1812 19.1 12 19.1C10.8188 19.1 9.43867 19.0726 8.0876 19.0344C5.23651 18.9537 3.81097 18.9134 2.90548 17.9819C2 17.0505 2 15.6028 2 12.7075Z"
                stroke="#fff"
                stroke-width="1.5"
              ></path>
            </svg>
          </a>
        </div>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

```

### style.css

```
* {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
}

html {
  width: 100%;
  height: 100%;
}

body {
  font-family: "Catamaran", sans-serif;
  font-size: 18px;
  color: #373737;
  line-height: 1.5;
}

img {
  max-width: 100%;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
}

@media screen and (max-width: 1140px) {
  .container {
    max-width: auto;
    width: 100%;
    padding: 0 20px;
  }
}

/* Typography */
h1,
h2,
h3 {
  margin: 0;
}

h2,
h3 {
  font-weight: 100;
  margin: 0 0 20px;
  line-height: 1;
}

h2 {
  font-size: 70px;
}

h3 {
  font-size: 30px;
}

p {
  margin: 0 0 10px;
}

/* Header and menu */
.header {
  padding: 30px 20px 0;
  display: flex;
  justify-content: space-between;
}

nav {
  text-align: right;
}

.menu {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  display: inline-block;
}

.menu a {
  padding: 10px 15px;
  color: #ffffff;
  text-decoration: none;
  font-size: 18px;
  border-bottom: 3px solid transparent;
  transition: border-bottom 0.5s ease-in;
}

.menu a:hover {
  border-bottom: 3px solid #bf0034;
}

.mobile-menu-icon {
  display: none;
}

@media screen and (max-width: 768px) {
  .menu {
    display: none;
  }

  .menu li {
    display: block;
  }

  .menu a {
    display: inline-block;
  }

  .mobile-menu-icon {
    display: inline-block;
  }

  .mobile-menu-icon:hover {
    cursor: pointer;
  }

  /* ikonka "x" ukryta na start */
  .icon-close {
    display: none;
  }

  /* zmiana ikony menu na "x" po kliknięciu */
  .mobile-menu-icon.opened .icon-menu {
    display: none;
  }

  .mobile-menu-icon.opened .icon-close {
    display: block;
  }

  .menu.opened {
    display: block;
    position: absolute;
    top: 60px;
    right: 20px;
    text-align: right;
  }
}

/* Hero section */
.hero-section {
  color: #ffffff;
  background: url("../images/hero-background-2.jpg") no-repeat;
  background-size: cover;
  background-position: bottom;
  width: 100%;
  height: 100vh;
}

.hero-logo {
  color: #bf0034;
}

.hero-title {
  font-weight: 900;
  font-size: 120px;
  line-height: 1;
  margin: 100px 0 40px;
}

.hero-lead {
  font-size: 22px;
  max-width: 45%;
  margin-bottom: 50px;
}

.hero-button {
  color: #ffffff;
  border: 3px solid #bf0034;
  text-decoration: none;
  padding: 8px 30px;
  font-size: 20px;
  text-transform: uppercase;
}

.hero-button:hover {
  background-color: #bf0034;
}

@media screen and (max-width: 768px) {
  .hero-title {
    font-size: 90px;
  }

  .hero-lead {
    max-width: 100%;
    font-size: 20px;
  }
}

/* Columns */
.columns-container {
  display: flex;
  justify-content: space-between;
}

.columns-2-container .column {
  width: 45%;
}

.columns-3-container {
  flex-wrap: wrap;
  row-gap: 25px;
}

.columns-3-container .column {
  width: 32%;
}

.columns-4-container .column {
  text-align: center;
  flex-basis: 25%;
}

@media screen and (max-width: 992px) {
  .columns-3-container {
    flex-direction: row;
  }

  .columns-3-container .column {
    width: 49%;
  }
}

@media screen and (max-width: 768px) {
  .columns-container {
    flex-direction: column;
  }

  .columns-2-container .column,
  .columns-3-container .column {
    width: 100%;
  }

  .columns-4-container {
    row-gap: 20px;
  }
}

/* Sections */
.section {
  padding: 100px 0;
}

.section-violet {
  background-color: #4f247c;
  color: #ffffff;
}

.section-pink {
  background-color: #bf0034;
  color: #ffffff;
}

.section-title {
  color: #bf0034;
}

/* About section */
.about-section {
  padding: 120px 0;
}

.about-image {
  text-align: center;
  position: relative;
  max-height: 550px;
}

.about-image img {
  max-height: 550px;
}

.about-image::before {
  content: "";
  border: 20px solid #4f247c;
  position: absolute;
  top: -35px;
  left: 20px;
  width: 366px;
  height: 550px;
  z-index: -2;
  box-sizing: border-box;
}

.about-image::after {
  content: "";
  background-color: #bf0034;
  position: absolute;
  top: 35px;
  right: 0px;
  width: 366px;
  height: 550px;
  z-index: -1;
  box-sizing: border-box;
}

@media screen and (max-width: 768px) {
  .about-text {
    margin-top: 60px;
  }
}

@media screen and (max-width: 450px) {
  .about-text {
    margin-top: 100px;
  }
}

/* Interests section */
.interests-section svg {
  border: 2px solid #bf0034;
  padding: 25px;
  border-radius: 50%;
}

.interest-name {
  margin: 20px 0;
}

.interest-text {
  padding: 0 10px;
  font-size: 14px;
}

/* Photos section */
.photos-title {
  text-align: center;
  color: #4f247c;
}

.photos-lead {
  text-align: center;
  max-width: 70%;
  margin: 0 auto;
  margin-bottom: 40px;
}

.photos-section figure {
  margin: 0;
}

.photos-section img {
  width: 100%;
  height: 240px;
  object-fit: cover;
}

.photos-section figcaption {
  font-size: 14px;
  margin-bottom: 0;
  text-align: center;
}

@media screen and (max-width: 768px) {
  .photos-lead {
    max-width: 100%;
  }

  .photos-section img {
    height: 350px;
  }
}

/* Quote section */
.quote-section {
  padding: 80px 0;
  overflow: hidden;
  position: relative;
}

.quote-section::after {
  content: "";
  background-color: #4f247c;
  position: absolute;
  right: -90px;
  bottom: -75px;
  width: 350px;
  height: 350px;
  z-index: 1;
  border-radius: 50%;
}

.quote-text {
  font-weight: 700;
  font-size: 40px;
  margin-bottom: 20px;
  z-index: 2;
  position: relative;
}

.quote-author {
  text-align: right;
  font-size: 14px;
  text-transform: uppercase;
  z-index: 2;
  position: relative;
}

@media screen and (max-width: 768px) {
  .quote-text {
    font-size: 30px;
  }
}

/* Contact section */
.contact-title {
  text-align: center;
  margin-bottom: 40px;
}

.contact-form {
  width: 50%;
  margin: 0 auto;
}

.contact-form label,
.contact-form input,
.contact-form textarea {
  display: block;
  width: 100%;
}

.contact-form input,
.contact-form textarea {
  border: 3px solid #4f247c;
  border-radius: 0;
  padding: 8px 15px;
  margin-bottom: 15px;
}
.contact-form label {
  padding-bottom: 5px;
}

.submit-button {
  color: #ffffff;
  background-color: #4f247c;
  border: 3px solid #4f247c;
  text-decoration: none;
  padding: 10px 40px;
  margin: 30px auto 0;
  display: block;
  font-size: 20px;
  text-transform: uppercase;
}

.submit-button:hover {
  color: #4f247c;
  background-color: #ffffff;
}

@media screen and (max-width: 768px) {
  .contact-form {
    width: 100%;
  }
}

/* Footer */
.footer {
  padding: 40px 0;
}

.social,
.copyright {
  width: 49%;
  display: inline-block;
}

.social {
  text-align: right;
}

.social a {
  display: inline-block;
  color: #ffffff;
  text-decoration: none;
  padding-left: 10px;
}

.copyright {
  font-size: 14px;
}

@media screen and (max-width: 768px) {
  .social,
  .copyright {
    width: 100%;
    display: block;
    text-align: center;
  }

  .social {
    margin-top: 20px;
  }
}

```
