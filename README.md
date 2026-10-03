# WOYO — téléchargements

Ce dépôt n'héberge **que** les applications WOYO à installer hors des stores.
Il ne contient aucun code : le code vit dans les dépôts privés de TAM.

Le site renvoie ici par des liens courts (`monwoyo.app/telecharger/…`). Si
l'hébergement change un jour, seuls ces liens du site changent de cible : les
liens donnés aux gens et les QR codes imprimés restent bons.

## Une « release » par application, avec un nom de fichier qui ne change jamais

| Release (étiquette) | Fichier | Pour qui |
|---|---|---|
| `woyo` | `woyo.apk` | les passagers (WOYO, Android 8 et plus) |
| `driver` | `woyo-driver.apk` | les motards et chauffeurs, téléphone récent |
| `driver` | `woyo-driver-32bits.apk` | les motards, ancien téléphone |
| `pro` | `woyo-pro.apk` | les loueurs de véhicules, téléphone récent |
| `pro` | `woyo-pro-32bits.apk` | les loueurs, ancien téléphone |

L'adresse d'un fichier ne bouge donc jamais, par exemple :
`https://github.com/fgh4gt4r5m-droid/woyo-telechargements/releases/download/pro/woyo-pro.apk`

## Publier une nouvelle version (DG ou équipe)

1. Dans Codemagic, télécharger l'APK du build (WOYO Pro et Driver :
   `app-arm64-v8a-release.apk` et `app-armeabi-v7a-release.apk`).
2. Le **renommer** comme dans le tableau : le lien du site en dépend.
3. Ici, onglet **Releases**, ouvrir la release de l'app, puis **Edit**.
4. Supprimer l'ancien fichier (croix), glisser le nouveau, et écrire dans la
   description la version et la date. Enregistrer avec **Update release**.
5. **Prévenir le site** (règle DG 2026-10-03) : mettre à jour le tableau « Les APK
   sont en ligne » de `woyo/docs/REPONSES-API-E.md` (taille, version, date). La
   page de téléchargement de monwoyo.app s'en sert.

Seuls des APK **signés en release** venant de Codemagic sont publiés ici,
jamais un build de debug.
