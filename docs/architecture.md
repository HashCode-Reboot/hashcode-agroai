# Architecture — AgroAI

```mermaid
flowchart TB
 U[Producteur] --> APP[Mobile / Web]
 IMG[Image] --> MM[Multimodal input]
 V[Voix] --> MM
 W[Météo] --> MM
 L[Localisation] --> MM
 APP --> MM
 MM --> K[Knowledge Base]
 MM --> AI[Models]
 K --> AI
 AI --> R[Recommandation]
 R --> C[Confiance]
 C --> H[Validation humaine si nécessaire]
 H --> U
```

## Principes

Séparer observations, prédictions et recommandations. Afficher l'incertitude. Tester les modèles sur les cultures, langues et conditions locales avant utilisation réelle.