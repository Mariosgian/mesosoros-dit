# Μέσος Όρος Πτυχίου ΕΚΠΑ

Υπολογισμός του **σταθμισμένου με ECTS** μέσου όρου πτυχίου για το Τμήμα Πληροφορικής & Τηλεπικοινωνιών του ΕΚΠΑ.

🔗 **Live:** _https://mesosoros-dit.pages.dev_

## Τι κάνει

- Ολόκληρο το πρόγραμμα σπουδών (μαθήματα + ECTS + τύπος) ήδη μέσα.
- Υπολογισμός μέσου όρου **live**, με τον επίσημο τύπο: `βαθμός × ECTS ÷ σύνολο ECTS`.
- Δείχνει και απλό (μη σταθμισμένο) μέσο όρο και τα ECTS που έχεις περάσει.
- **Στόχος μέσου όρου:** σου λέει τι βαθμό χρειάζεσαι στα υπόλοιπα μαθήματα.
- Αναζήτηση μαθήματος, προσθήκη δικών σου μαθημάτων.
- **Dark / light theme** με απομνημόνευση επιλογής.
- Οι βαθμοί αποθηκεύονται **τοπικά** στον browser (localStorage) — τίποτα δεν ανεβαίνει σε server.

## Tech

- Single-file, **vanilla HTML/CSS/JS** — μηδέν dependencies, μηδέν build step.
- Offline-first (localStorage), responsive, προσβάσιμο (ARIA labels, keyboard navigation).
- Privacy-first analytics με Cloudflare Web Analytics (χωρίς cookies).

## Author

Built by **[Marios Giannoulis](https://www.linkedin.com/in/marios-giannoulis-129576289/)**
