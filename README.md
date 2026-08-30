# Portal d'Informes GIFF (Fedefarma) — versió pública

Aquest repositori conté **només** el resultat final del Portal d'Informes:
- `Portal_Informes.html` — el portal en si (autocontingut, carrega els CSV automàticament via `fetch()` quan es serveix per web).
- `Datos_Portal_Operaciones.csv` / `Datos_Portal_Stock.csv` — les dades ja processades que consumeix el portal.

Es publica via **GitHub Pages** perquè hi hagi una URL estable accessible per a tothom amb l'enllaç.

Els scripts font, les extraccions crues d'Informix i la documentació interna de l'ERP **no viuen aquí** —
es mantenen al repositori privat [`PortalInformesOps`](https://github.com/fmiret/PortalInformesOps).
Aquest repositori es sobreescriu automàticament cada dia des d'allà.
