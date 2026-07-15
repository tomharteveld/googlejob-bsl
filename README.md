# Medische Banenbank – Google Jobs dashboard

Statische, zelfstandige dashboardwebsite voor GitHub en Vercel. De actuele CSV-data en het logo zijn in `index.html` ingebed; er zijn geen externe databronnen of buildstappen nodig.

## Publiceren via GitHub en Vercel

1. Maak een nieuwe GitHub-repository.
2. Upload `index.html`, `vercel.json` en dit `README.md` naar de hoofdmap van de repository.
3. Kies in Vercel **Add New > Project** en importeer de GitHub-repository.
4. Laat **Framework Preset** op **Other** staan en klik op **Deploy**.

## Data bijwerken

Open het dashboard lokaal, laad de drie nieuwe CSV-exports via **CSV laden** en klik op **Bijgewerkte HTML downloaden**. Vervang daarna het bestaande `index.html` in GitHub; Vercel publiceert de wijziging automatisch.

Gebruik bij voorkeur tegelijk:

- `keywords.csv`
- `keyword_results.csv`
- `job_results.csv`

Het dashboard kiest automatisch de nieuwste run die bij de vacaturedata hoort. DataForSEO-regels met `Task In Queue` worden als wachtrij getoond en niet als gemiste zichtbaarheid meegeteld.
