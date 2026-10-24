# 🎬 Moebius Film Generator — 100 Images

Générateur de film cinématique à partir d'images de référence, en style **Moebius** (comics SF franco-belge des années 70).

![Status](https://img.shields.io/badge/status-ready-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Zero deps](https://img.shields.io/badge/dependencies-0-success)

## ✨ Fonctionnalités

- **Pipeline img→txt→img** : extraction du contenu narratif → génération de 100 frames cinématiques
- **Style Moebius** : ligne claire, hachures fines, palette pastel poussiéreuse
- **Multi-Keys API** : jusqu'à 10 clés en rotation adaptative avec failover automatique
- **Workers parallèles** : 6 générations simultanées (configurable)
- **Interface 100% navigateur** : aucun serveur requis, aucune dépendance
- **Timeline film** : visualisation des 100 frames comme une pellicule
- **Console intégrée** : logs détaillés + export

## 🚀 Utilisation

### En local
1. Télécharge `index.html`
2. Ouvre-le dans ton navigateur (double-clic)
3. C'est tout ✅

### Via GitHub Pages
👉 **https://nivoit.github.io/moebius-film-generator/**

## 🔑 Configuration

| Champ | Description |
|-------|-------------|
| **Clés API** | Une clé par ligne (format `sk-...`) — max 10 |
| **Images de référence** | 1 à N images (sujets du film) |
| **Longueur du film** | 10 à 200 frames (défaut : 100) |

### Endpoints utilisés
- `https://apihub.agnes-ai.com/v1/chat/completions` (vision — img→txt)
- `https://apihub.agnes-ai.com/v1/images/generations` (génération — txt→img)

### Modèles
- Texte/Vision : `agnes-2.5-flash`
- Image : `agnes-image-2.5-flash`

## 🎨 Style Moebius

- Contours à l'encre « ligne claire » ininterrompus
- Hachures fines pour la texture
- Palette pastel poussiéreuse (ocre pâle, rose, turquoise doux)
- Perspective atmosphérique, surréalisme

## ⚠️ Notes

- Les clés API sont stockées **uniquement en mémoire** (jamais persistées)
- Aucun cookie, aucun tracking
- Projet = fichier HTML autonome (zero dependency)

## 📄 Licence

MIT — voir [LICENSE](LICENSE)

## 🙏 Crédits

- Style visuel inspiré de **Jean Giraud (Moebius)** et du magazine **Métal Hurlant**
- API : [Agnes AI](https://agnes-ai.com)
