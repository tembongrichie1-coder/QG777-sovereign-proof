# 🛡️ QG777 Sovereign Core v4.3

**Le premier système de preuve inviolable - La Défense, Paris**

> "Une ronde sans preuve est une ronde qui n'a jamais existé." - Richie Ahmed Tembong

### Le Probleme
Feuilles de ronde falsifiables. Aucune preuve.

### Solution QG777
Chaque ronde scellée SHA-256 + horodatage blockchain. Inviolable.

### Stack v4.3
- FastAPI + SQLAlchemy
- SHA-256 auto à chaque POST/PUT
- Audit: /parcours/verifier-integrite
- Client CLI + Export JSON juridique
- Auth X-API-KEY via .env

### Installation
pip install fastapi uvicorn sqlalchemy pydantic python-dotenv requests
uvicorn main:app --reload
python client.py verifier

### Auteur
Richie Ahmed Tembong - Fondateur QG777 Systems
