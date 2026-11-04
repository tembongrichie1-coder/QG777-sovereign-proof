# 🛡️ QG777 Sovereign Core v5.0 - Mesh Sovereign

**Le premier système de preuve inviolable maillé - La Défense, Paris**

> "Une ronde sans preuve est une ronde qui n'a jamais existé." - Richie Ahmed Tembong

### 🔗 Le Problème
Feuilles de ronde falsifiables. Aucune preuve. Pas de traçabilité terrain.

### ⚡ Solution QG777 v5.0
1.  **v4.3 Core:** Chaque ronde scellée SHA-256 + horodatage blockchain de poche. Inviolable.
2.  **v5.0 Mesh (NOUVEAU):** Daemon souverain maillé.
    - Découverte automatique Multicast UDP 239.255.255.250:5007
    - Synchronisation SQLite automatique entre pairs
    - Signature Ed25519 de chaque paquet
    - Ancrage Blockchain on-chain via Web3 `anchorBatch`

### 🧱 Stack v5.0
- **API:** FastAPI + SQLAlchemy + Audit `/parcours/verifier-integrite`
- **Mesh:** asyncio + aiosqlite + Multicast + Ed25519
- **Blockchain:** Web3.py - Ancrage de batch SHA-256 sur EVM
- **Client:** CLI `python client.py verifier` + Export JSON juridique
- **Secu:** Auth X-API-KEY via `.env` + `.gitignore` blindé

### 🚀 Installation v5.0
```bash
pip install -r requirements.txt
# Core v4.3
uvicorn main:app --reload
python client.py verifier

# Daemon Mesh v5.0 (NOUVEAU)
python sovereign_core_daemon.py
# Le daemon écoute sur 127.0.0.1:9999, découvre les pairs en multicast
