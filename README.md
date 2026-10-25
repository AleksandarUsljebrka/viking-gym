# Viking Gym

Početna strana za Viking Gym, teretanu sa pet sala u Beogradu i Novom Sadu.

Statičan sajt: jedan HTML fajl i slike. Nema build koraka, nema zavisnosti. Fontovi se učitavaju sa Google Fonts.

## Struktura

```
index.html             stranica, CSS i JavaScript
assets/favicon.svg     ikonica u tabu pregledača
assets/img/hero.jpg    pozadina naslovne sekcije
assets/img/sala-tegovi.jpg    slika u sekciji O nama
assets/img/sala-prozori.jpg   pozadina iza kontakt forme
assets/img/trener.jpg  fotografija trenera
.nojekyll              GitHub Pages servira fajlove bez obrade
```

## Objava na GitHub Pages

1. Napravi novi repozitorijum na GitHub-u, na primer `viking-gym`.
2. Pošalji ove fajlove u granu `main`:

   ```
   git init
   git add .
   git commit -m "Viking Gym početna strana"
   git branch -M main
   git remote add origin https://github.com/KORISNIK/viking-gym.git
   git push -u origin main
   ```

3. Na GitHub-u otvori **Settings → Pages**.
4. Pod **Build and deployment** izaberi **Deploy from a branch**, granu `main` i folder `/ (root)`, pa klikni **Save**.
5. Posle minut-dva sajt je na `https://KORISNIK.github.io/viking-gym/`.

Za svoj domen (na primer `vikinggym.rs`) upiši ga u **Settings → Pages → Custom domain** i podesi DNS kod registra domena.

## Lokalni pregled

Otvori `index.html` u pregledaču, ili pokreni mali server u ovom folderu:

```
npx http-server -p 8080
```

## Pre objave zameni

Ovo su privremeni podaci:

- **Cene** u cenovniku (3.900, 4.900, 16.000 i 2.200 RSD)
- **Adrese i radno vreme** sala u sekciji Lokacije. Ulice postoje, brojevi su izmišljeni.
- **Telefon, email i Instagram** u kontakt sekciji
- **Imena, iskustvo i edukacija trenera** i njihove fotografije. Sada je ista fotografija na sve četiri kartice.
- **Fotografije sala.** `sala-tegovi.jpg` i `sala-prozori.jpg` su sa Pexelsa, a `hero.jpg` je generisana AI slika. Najbolje ih je zameniti fotografijama vaših sala.

Forma za upis proverava polja, ali podatke ne šalje nigde. Za pravo slanje poveži je sa servisom kao što je Formspree, ili sa svojim bekendom.
