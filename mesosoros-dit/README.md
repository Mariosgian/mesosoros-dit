# Μέσος Όρος Πτυχίου ΕΚΠΑ

Υπολογισμός του **σταθμισμένου με ECTS** μέσου όρου πτυχίου για το Τμήμα Πληροφορικής & Τηλεπικοινωνιών του ΕΚΠΑ.

🔗 **Live:** _https://ekpa-gpa.pages.dev_

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

## Deploy σε Cloudflare Pages

1. Ανέβασε τον φάκελο σε GitHub repo.
2. Cloudflare dashboard → **Workers & Pages** → *Create* → *Pages* → *Connect to Git*.
3. Διάλεξε το repo. **Build command:** (κενό). **Output directory:** `/`.
4. *Deploy* → live στο `<name>.pages.dev` με δωρεάν HTTPS.
5. Κάθε `git push` κάνει αυτόματο re-deploy (CI/CD).

### Analytics

Cloudflare → **Web Analytics** → πρόσθεσε το site → αντίγραψε το token → ξεσχολίασε το beacon
`<script>` στο τέλος του `index.html` βάζοντας το token σου.

## Author

Built by **[Marios Giannoulis](https://www.linkedin.com/in/marios-giannoulis-129576289/)**
