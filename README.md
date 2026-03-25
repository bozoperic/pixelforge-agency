# 💻 PixelForge Digital Agency — Grupni projekt

**Grupa B · 4 učenika · Bootstrap završni projekt**

---

## 📋 O projektu

Izrađujete web stranicu za fiktivnu digitalnu agenciju **PixelForge**.
Stranica mora izgledati profesionalno i moderno, kao da je napravljena za pravog klijenta.

> ⚠️ **Napomena:** Ovaj projekt koristi isključivo HTML, CSS i Bootstrap.
 sve interaktivnosti (modal, hamburger, accordion)
> rade kroz Bootstrap `data-bs-*` atribute.

---

## 👥 Podjela uloga i zadataka

| Uloga | Učenik | Branch | Zadatak |
|-------|--------|--------|---------|
| **Lead Developer** | *(upišite ime)* | `feature/hero-navigacija` + `feature/tim-kontakt` | Navbar, Hero, Tim sekcija, Kontakt forma, koordinacija |
| **UI Developer 1** | *(upišite ime)* | `feature/usluge` | Sekcija usluga s 6 kartica |
| **UI Developer 2** | *(upišite ime)* | `feature/portfolio` | Portfolio galerija s modalima |
| **CSS Developer** | *(upišite ime)* | `feature/css-footer` | Cijeli `style.css`, varijable, footer |

> **CSS Developer** postavlja `:root` varijable i boje **prvi** i mergea ih u main — ostali čekaju taj merge kako bi znali koje klase koristiti.

---

## 🚀 Git workflow — korak po korak

### Početak rada

```bash
# 1. Kloniraj repo
git clone https://github.com/[username]/pixelforge-agency.git
cd pixelforge-agency

# 2. Napravi branch
git checkout -b feature/tvoj-zadatak

# 3. Provjeri na kojoj si grani
git branch
```

### Tijekom rada

```bash
# Redoviti commitovi — svaki logički korak poseban commit
git add .
git commit -m "Opisna poruka — što si napravio"

# Push na GitHub (prvi put s -u)
git push -u origin feature/tvoj-zadatak

# Svaki sljedeći put:
git push
```

### Sync s mainom — OBAVEZNO svakih 20-30 minuta

```bash
git checkout main
git pull
git checkout feature/tvoj-zadatak
git merge main
# Ako nastane conflict → rješavaj zajedno s Lead Devom
```

### Pull Request

1. GitHub → **Compare & pull request**
2. Reviewer: Lead Developer (obavezan)
3. Opis PR-a: što si napravio, što je testirano
4. Čekaj review prije mergea

---

## ⚠️ Pravila rada

1. **CSS Dev postavlja `:root` varijable prvi** — ostali čekaju taj merge
2. **Nikad direktno na main**
3. **Opisne commit poruke** (`"WIP"` nije prihvatljivo)
4. **Konflikte u `index.html`** rješava Lead Developer s osobom čiji je PR
5. **Svaka osoba ima minimalno 8 commitova** na kraju projekta
6. **Bez JavaScripta** — sve interaktivnosti kroz Bootstrap klase i atribute

---

## 📁 Struktura projekta

```
pixelforge-agency/
├── index.html       ← svi dodaju svoje sekcije ovdje
├── css/
│   └── style.css    ← vlasnik: CSS Developer
├── img/
└── README.md        ← popunite imenima!
```

---

## ✅ Zahtjevi — što mora biti implementirano

### Obavezno:
- [ ] Navbar (sticky, s hamburgerom na mobitelu, `navbar-expand-lg`)
- [ ] Hero sekcija (min-height 100vh, tamna pozadina)
- [ ] 6 kartica usluga u gridu (`col-md-4`) s ikonom, opisom i `badge`-om
- [ ] 6 portfolio kartica — svaka ima gumb koji otvara modal s opisom projekta
- [ ] Tim sekcija (min. 3 člana) — slika, ime, pozicija, opis
- [ ] Kontakt forma (min. 4 polja)
- [ ] Footer s logom, linkovima i copyright retkom
- [ ] Custom CSS — promijenjena primarna boja i font, min. 3 custom stila
- [ ] Responzivno na 375px
- [ ] Min. 8 commitova po osobi s opisnim porukama
- [ ] Svi PR-ovi pregledani i mergani

### Bonus (samo Bootstrap, bez JS):
- [ ] `accordion` za FAQ sekciju (pitanja o procesu suradnje, cijenama...)
- [ ] `badge` oznake na portfolio karticama (kategorija: Web / Brand / Print)
- [ ] `card-header` s kategorijom na karticama usluga
- [ ] Dismissible `alert` s aktualnom promocijom
- [ ] `list-group` za popis prednosti svake usluge
- [ ] `nav-pills` za vizualni prikaz kategorija portfolia (samo izgled, bez filtriranja)

---

## 🗓️ Vremenski okvir

| Faza | Što | Rok |
|------|-----|-----|
| Setup | Clone, branch, dogovor o bojama | Prvih 15 min |
| CSS Dev | `:root` varijable → merge → ostali počinju | Sat 1, prvih 30 min |
| Razvoj | Svaki na svom branchu | Sat 1 + Sat 2 |
| Integracija | PR-ovi, review, merge, konflikti | Zadnjih 30 min |
| Prezentacija | Demo | Kraj |

---

## 🎨 Smjernice dizajna

- **Paleta:** tamno plava ili crna + električna akcent boja (plava, ljubičasta ili zelena)
- **Fontovi:** Space Grotesk (naslovi) + Inter (tijelo) — već učitani u CSS-u
- **Stil:** moderan, tehnološki, minimalistički
- **Slike:** `https://picsum.photos/seed/[naziv]/600/400`

---

*Projekt se predaje kao GitHub repo link. README mora biti popunjen imenima.*
