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
This was a team project, and we collaborated across the whole system. I worked mainly on three areas:

**Authentication and account access**
- Login and registration screens for contractors and suppliers, with form validation (password policy, confirm-password check)
- Role-based access, so contractors, suppliers and admins each see only what they should

**Listings**
- Browsing and searching listings, and the listing detail view
- Creating and editing listings as a supplier
- Working with the API endpoints and data models behind listings

**Admin dashboard and reports**
- Admin dashboard summary and reports for managing the platform

Working in a team also taught me to use Git for collaboration, follow shared coding conventions, and integrate my work with teammates' parts of the app.

## Running it locally
Each folder has its own setup notes.
- **API:** see `api/SECRETS_SETUP.md` (add your own connection string and keys with `dotnet user-secrets`; no real secrets are stored in this repo).
- **Web / mobile:** `npm install`, then `ng serve` (web) or `ionic serve` (mobile).
