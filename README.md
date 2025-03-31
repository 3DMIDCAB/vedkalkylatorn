# Vedomräknare – Version 2

Det här är version 2 av ett enkelt och smart verktyg för att räkna om vedvolymer. Denna version inkluderar nu **vedlängd som inmatning**, vilket ger mer noggranna beräkningar av fast volym.

## 🪵 Funktioner

- Omvandling mellan:
  - **Stjälpt mått (m³s)** – löst hälld ved
  - **Staplat mått (m³t)** – staplad ved
  - **Fast mått (m³f)** – endast trävolym
- Användaren kan mata in **valfri vedlängd (i cm)** mellan 20–60 cm
- Omräkningsfaktorer anpassas automatiskt beroende på vedlängden
- Enkel att använda direkt i webbläsaren

## 🔧 Omräkningslogik

Omräkning mellan måtten bygger på standardfaktorer:
- 1 staplad m³ ≈ 1,4 stjälpta m³
- Fast volym beräknas utifrån vedlängd enligt följande interpolering:

| Vedlängd | Faktor staplat → fast |
|----------|------------------------|
| 25 cm    | 0.72                   |
| 30 cm    | 0.70                   |
| 40 cm    | 0.68                   |
| 50 cm    | 0.66                   |

## ✅ Användning

1. Öppna `vedomraknare-v2.html` i en webbläsare.
2. Fyll i:
   - Ett av måtten (stjälpt, staplat eller fast)
   - Valfri vedlängd (t.ex. 30 cm)
3. Verktyget räknar ut de andra två måtten automatiskt.

## 📌 Exempel

Om du matar in:

- Vedlängd: `30 cm`
- Stjälpt: `40 m³s`

Då får du:

- Staplat: `28.57 m³t`
- Fast: `20.00 m³f`

## 📤 Publicering

Versionen är anpassad för publicering via t.ex. [Netlify Drop](https://app.netlify.com/drop) eller GitHub Pages.

## 👤 Skapare

Verktyget är skapat av **Patrik Åkerlöf**, Vallstena på Gotland  
📧 Kontakt: `patrik.akerlof@gmail.com`

## 📜 Licens

Fritt att använda och dela för privat bruk. Vid kommersiell användning – kontakta upphovsmannen.
