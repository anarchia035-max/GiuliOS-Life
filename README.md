# LifeOS - Premium Edition

Sito statico PWA minimal per uso personale.

Deployment rapido (consigliato): collegare il repository GitHub a Render per deploy automatico.

Passaggi rapidi per pubblicare (locale):

1. Inizializza e fai commit locale (già fatto):

```bash
git init
git add .
git commit -m "Initial PWA: manifest, sw, offline, deploy configs"
git branch -M main
```

2. Crea il repo GitHub (pubblico) e push:

```bash
# usando gh CLI (raccomandato):
gh repo create YOUR_USER/YOUR_REPO --public --source=. --remote=origin --push

# oppure via web: crea repo e poi:
git remote add origin git@github.com:YOUR_USER/YOUR_REPO.git
git push -u origin main
```

3. Su Render: crea nuovo servizio -> collega GitHub -> seleziona `main` -> Static Site -> `staticPublishPath` `/`.

Note:
- iPhone richiede HTTPS e che il sito sia servito via HTTPS per installare la PWA.
- puoi sostituire le icone remote con file locali in `icons/` e aggiornare `manifest.json`.
# GiuliOS-Life
