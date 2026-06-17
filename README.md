# Testspecialist.nl — Website

Statische website voor [Testspecialist.nl](https://testspecialist.nl), een bureau voor professionele softwaretestdiensten.

## Pagina's

| Pagina | Bestand | URL |
|--------|---------|-----|
| Home | `index.html` | `/` |
| Diensten | `diensten.html` | `/diensten` |
| Team | `team.html` | `/team` |
| Contact | `contact.html` | `/contact` |

## Techniek

- Puur HTML en CSS, geen frameworks of build-stap
- `.htaccess` verbergt de `.html` extensie in URLs
- Afbeeldingen staan in de `images/` map

## Deployment

Elke push naar `main` deployt automatisch via GitHub Actions naar de FTP-server.

De workflow staat in [.github/workflows/deploy.yml](.github/workflows/deploy.yml).

### Benodigde GitHub Secrets

| Secret | Omschrijving |
|--------|-------------|
| `FTP_SERVER` | Hostnaam van de FTP-server |
| `FTP_USERNAME` | FTP-gebruikersnaam |
| `FTP_PASSWORD` | FTP-wachtwoord |

## Lokaal bekijken

Geen build-stap nodig. Open `index.html` direct in een browser.
