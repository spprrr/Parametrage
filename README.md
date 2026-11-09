# Fiches Paramétrage – Projet Android

Ce dossier contient votre application HTML d'origine intégrée dans un projet Capacitor 7.

## Création du projet Android dans GitHub Codespaces

Ouvrez ce dossier dans un Codespace, puis exécutez dans le terminal :

```bash
npm install
npx cap add android
npx cap sync android
```

Le dossier `android` sera créé automatiquement.

## Générer l'APK

Dans Codespaces, vérifiez qu'un JDK 21 et Android SDK sont disponibles, puis :

```bash
cd android
./gradlew assembleDebug
```

L'APK debug sera normalement créé ici :

`android/app/build/outputs/apk/debug/app-debug.apk`

## Fonctionnalités conservées

- Fiches de paramétrage et champs existants
- Photos liées aux fiches, stockées dans IndexedDB
- Affichage agrandi des photos au toucher
- Sauvegarde et restauration JSON avec photos
- Recherche, modification, duplication et suppression

## Important – sauvegarde des données

Les données de l'application sont conservées localement sur l'appareil. Exportez régulièrement une sauvegarde depuis le bouton « Sauvegarde » et gardez le fichier JSON dans un emplacement sûr.

Ce ZIP contient le projet source prêt à initialiser avec Capacitor ; il ne contient pas encore le dossier Android généré ni un APK compilé.
