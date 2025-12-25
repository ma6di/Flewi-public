# Flewi

Flewi is a language-learning web app with flashcards and spaced repetition.

## Tech stack

- Frontend: React (Vite), Tailwind CSS
- Backend: FastAPI (Python)
- Database: PostgreSQL
- Cache/queues: Redis
- Reverse proxy / TLS: Caddy (in production)
- Containers: Docker / Docker Compose

## What you can do

- Create and review flashcards with spaced repetition
- Organize words into boxes/collections
- Track learning progress and activity
- Use pronunciation / audio (depends on your configured TTS provider)
- Install as a PWA (add to home screen)

## Run (Docker)

```bash
git clone https://github.com/ma6di/Flewi.git
cd Flewi

docker compose up -d
```

Open http://localhost

## Install (PWA)

Flewi supports installation as a Progressive Web App (PWA), so you can add it to your home screen and use it like a native app.

- iOS (Safari): open the site → Share → Add to Home Screen
- Android (Chrome): open the site → menu (⋮) → Install app / Add to Home screen
- Desktop (Chrome/Edge): click the install icon in the address bar (if shown)

## Screenshots

Add images to a folder (for example `docs/screenshots/`) and link them here.


Home (desktop)

<img src="https://github.com/user-attachments/assets/e1debb36-3dda-4070-8121-8af08034e757" width="900" alt="Home" />

Flashcards (desktop)

<img src="https://github.com/user-attachments/assets/f0c35fa0-5899-4b35-8cfa-ea4e7840206a" width="900" alt="Flashcards" />

Stats (desktop)

<img src="https://github.com/user-attachments/assets/dfff228d-3ed6-435c-863c-45d0873262ad" width="900" alt="Stats" />

Focus Mode (mobile)                                                  Decks (mobile)

<img src="https://github.com/user-attachments/assets/28230581-3769-48e0-87f8-132bfb97e929" width="360" alt="Focus Mode" />          <img src="https://github.com/user-attachments/assets/79600cdc-0ba7-4684-a21b-ec41b68ffd15" width="360" alt="Decks" />
## Useful links

- API docs (after start): http://localhost:8000/docs
- Deployment: [DOCKER_DEPLOYMENT.md](DOCKER_DEPLOYMENT.md)

## Troubleshooting

```bash
docker compose logs -f
docker compose restart
```
