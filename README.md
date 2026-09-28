# EquaMeridian Marketplace

A group project (Team 39, University of Pretoria): a marketplace where **Contractors** find and book equipment/services from **Suppliers**, with quotes, lease agreements, invoices, payments and dispute handling. It ships as three connected parts.

## Live demo
- Web app: https://equameridian-hub.onrender.com/
- API docs (Swagger): https://equameridian-api.onrender.com/swagger/index.html

*(Hosted on a free tier, so the first load can take about a minute while the servers wake up.)*

## Repository structure
| Folder | What it is | Tech |
|---|---|---|
| `api/` | Backend REST API | ASP.NET Core, C#, PostgreSQL, JWT auth, Docker, unit tests |
| `web-hub/` | Web application for contractors, suppliers and admins | Angular |
| `mobile-app/` | Mobile app for contractors and suppliers | Ionic, Angular, Capacitor |

## Main features
- Browse listings, request quotes or book instantly, cart and checkout
- Quotations, lease agreements, invoices and payments (PayFast card payments, EFT with proof of payment)
- Bookings, disputes, reviews, messaging and notifications
- Admin tools: audit log, reports, backups, data export, content rules, fee configuration

## My contribution
> **TODO: replace this section with your own words.** Say which parts YOU built (for example: "I built the booking flow in the API and the invoices screens in the web app"). Recruiters read this section closely.

## Running it locally
Each folder has its own setup notes.
- **API:** see `api/SECRETS_SETUP.md` (add your own connection string and keys with `dotnet user-secrets`; no real secrets are stored in this repo).
- **Web / mobile:** `npm install`, then `ng serve` (web) or `ionic serve` (mobile).

## Team
> **TODO: list your teammates' names (with their permission).**
