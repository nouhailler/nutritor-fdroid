# 📦 Nutritor — Dépôt F-Droid

Dépôt F-Droid officiel de [Nutritor](https://github.com/nouhailler/nutritor), l'assistant nutritionnel & digestif pour Android.

[![F-Droid](https://img.shields.io/badge/F--Droid-Dépôt%20officiel-1976D2?style=for-the-badge&logo=f-droid)](https://nouhailler.github.io/nutritor-fdroid/repo)
[![Download APK](https://img.shields.io/github/v/release/nouhailler/nutritor?label=Dernière%20version&logo=android&color=3F5A3A&style=for-the-badge)](https://github.com/nouhailler/nutritor/releases/latest)

---

## 📲 Installer Nutritor via F-Droid

### Étape 1 — Installer F-Droid

Si tu n'as pas encore F-Droid sur ton appareil Android :

👉 [Télécharger F-Droid](https://f-droid.org)

### Étape 2 — Ajouter le dépôt Nutritor

Dans F-Droid : **Paramètres → Dépôts → +** et coller l'URL :

```
https://nouhailler.github.io/nutritor-fdroid/repo
```

Ou scanner ce QR code directement depuis F-Droid :

![QR Code](docs/qrcode.png)

### Étape 3 — Installer Nutritor

1. Rafraîchir les dépôts dans F-Droid (tirer vers le bas)
2. Chercher **Nutritor**
3. Installer

---

## 🔐 Vérification de l'authenticité

Pour vérifier que l'APK provient bien de ce dépôt officiel, contrôle l'empreinte de la clé de signature :

**SHA-256 :**
```
58:50:D1:AE:EF:21:50:39:71:DB:8F:59:E0:46:35:CC:9D:5F:98:55:B0:5E:43:4C:9A:B2:D9:09:4A:D3:33:33
```

Dans F-Droid, cette empreinte est visible dans **Paramètres → Dépôts → Nutritor**.

---

## 🔄 Mises à jour

Les mises à jour sont publiées automatiquement à chaque nouvelle release de Nutritor. F-Droid te notifiera dès qu'une mise à jour est disponible.

Pour mettre à jour manuellement : **F-Droid → Mises à jour → Nutritor**.

---

## 📱 À propos de Nutritor

Nutritor est un assistant nutritionnel & digestif conçu pour les personnes avec SII, intolérances alimentaires, ou simplement curieuses de ce qu'elles mangent.

**Fonctionnalités principales :**
- Journal alimentaire avec suivi des macros
- Base CIQUAL/ANSES complète (47 000+ aliments)
- Protocole Low FODMAP intégré
- Scanner de codes-barres (Open Food Facts)
- Statistiques hebdomadaires et mensuelles
- 100 % hors-ligne, sans compte, sans pub

👉 [Voir le projet complet](https://github.com/nouhailler/nutritor)

---

## 🛠️ Structure du dépôt

```
nutritor-fdroid/
├── repo/                  # Index F-Droid et APKs
│   ├── index-v2.json      # Index signé (F-Droid 1.5+)
│   ├── index-v1.jar       # Index signé (F-Droid legacy)
│   └── nutritor-*.apk     # APKs des versions publiées
├── metadata/
│   └── com.nutritor.app.yml  # Métadonnées de l'application
└── .github/workflows/
    └── fdroid-update.yml  # Auto-update à chaque release
```

---

## ⚠️ Note de sécurité

Le fichier `keystore.p12` (clé de signature du dépôt) n'est **pas** inclus dans ce repo. Il est stocké de manière sécurisée via les secrets GitHub Actions.

---

*Dépôt maintenu par [@nouhailler](https://github.com/nouhailler) · Mis à jour automatiquement via GitHub Actions*
