# Om mig – Oliver Tham

Min personliga om-mig-sida, byggd under kursen på UX Engineer-utbildningen på Chas Academy.
Sidan presenterar vem jag är, vad jag kan, min bakgrund och hur man når mig.

Byggd med HTML, CSS och JavaScript, utan ramverk.

## Innehåll

- Profil med namn, kort beskrivning och länkar till GitHub och LinkedIn
- Flikar: Om mig, Skills, Intressen och Kontakt
- Tidslinje över min utbildning och erfarenhet

## Interaktioner

- **Mörkt läge** – knappen växlar klassen `dark` på `<html>`. Valet sparas i `localStorage`, och första gången följer sidan systemets inställning.
- **Flikar** – visar en panel i taget. Fungerar med mus och med piltangenter, Home och End.
- **Läs mer / Visa mindre** – ett `if...else` visar eller döljer extra text och byter knappens text.
- **Skrivmaskin** – texten "Jag är …" skrivs och suddas fram mellan olika ord.
- **Tidslinje** – punkterna tonar in när de scrollas fram (`IntersectionObserver`).
- **Kontaktformulär** – kontrollerar att alla fält är ifyllda och visar ett meddelande.

## Tillgänglighet

- Semantisk HTML: `header`, `nav`, `main`, `section`, `footer`, och rubriker i ordning
- Allt klickbart är `button` eller `a`
- Flikarna använder `role="tab"`, `aria-selected` och `aria-controls`
- `aria-expanded` på Läs mer-knappen och `aria-pressed` på knappen för mörkt läge
- Formulärmeddelandet har `role="status"` så att skärmläsare läser upp det
- Skrivmaskinstexten döljs för skärmläsare, som i stället får hela meningen
- Tydlig fokusmarkering (`:focus-visible`) för tangentbordsanvändare
- Animationerna stängs av för den som valt reducerad rörelse (`prefers-reduced-motion`)
- Alt-text på bilderna, `lang="sv"` och responsiv layout från mobil till desktop
