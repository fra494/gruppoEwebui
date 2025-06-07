# 🐳 Setup del Progetto con Docker e Let's Encrypt

Questa repository contiene un ambiente Docker per l'esecuzione del progetto con supporto a HTTPS tramite Let's Encrypt.

## ✅ Requisiti

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## 🚀 Istruzioni per l'avvio

Segui questi passaggi per avviare correttamente l'ambiente:

### 1. Configura l’ambiente

Copia il file `.env-test` e rinominalo in `.env`, poi modifica le variabili al suo interno secondo le tue esigenze:

```bash
cp .env-test .env
nano .env
```

### 2. Genera i certificati SSL

Esegui lo script per abilitare i certificati HTTPS tramite Let's Encrypt:


```bash
./enable_letsencrypt.sh
```

### 3. Avvia Docker Compose

Avvia i container con:


```bash
docker compose up -d
```
