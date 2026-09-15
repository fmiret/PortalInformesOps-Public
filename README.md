# Portal d'Informes GIFF (Fedefarma) — versió pública

Aquest repositori conté **només** el resultat final del Portal d'Informes:
- `Portal_Informes.html` — el portal en si (autocontingut, carrega els CSV automàticament via `fetch()` quan es serveix per web). Conté els informes **Informe Diari**, **Dossier Mensual** i **Documentació**.
- `Datos_Portal_Operaciones.csv` / `Datos_Portal_Stock.csv` — les dades ja processades que consumeix el portal.
- `Stock_Magatzem_Laboratori_Compte.html` — informe "Stock per Magatzem/Laboratori/Compte", publicat des del 15/09/2026 com a **fitxer independent** (ja no va embegut dins `Portal_Informes.html`). Intenta carregar `Datos_Portal_Stock.csv` automàticament; si no el troba, es pot carregar manualment amb el botó de la pròpia pàgina.
- `Seguimiento_Encajadora_CMC.html` — informe "Seguiment encaixadora CMC", també publicat des del 15/09/2026 com a **fitxer independent**. Autocontingut: l'usuari hi arrossega el seu propi Excel `ff_robot_log` exportat des d'Axional, no depèn de cap CSV d'aquest repositori.

Aquests 2 informes es van treure del `Portal_Informes.html` (petició de Francesc) perquè ara es mostren
com a entrades pròpies dins **Sistema Central de Reporting** (`Dev/Sistema_Central_Reporting.html`, al PC
de Francesc), que enllaça directament a aquests fitxers.

Es publica via **GitHub Pages** perquè hi hagi una URL estable accessible per a tothom amb l'enllaç.

Els scripts font, les extraccions crues d'Informix i la documentació interna de l'ERP **no viuen aquí** —
es mantenen al repositori privat [`PortalInformesOps`](https://github.com/fmiret/PortalInformesOps).
Aquest repositori es sobreescriu automàticament cada dia des d'allà.
