# HelloToast — Application Android

Une application Android simple démontrant l'utilisation des **messages Toast** et d'un **compteur interactif**.

---

## Démonstration vidéo

<!-- Remplace ce bloc par ta vidéo après l'avoir uploadée sur GitHub ou YouTube -->

https://github.com/TON_USERNAME/TON_REPO/assets/TON_ID/ta-video.mp4

> Pour ajouter ta vidéo : va sur GitHub → ouvre une Issue → glisse ta vidéo dedans → copie le lien généré → colle-le ici à la place du lien ci-dessus.

[Running Devices - HelloToast 2026-04-09 22-02-37.zip](https://github.com/user-attachments/files/26614821/Running.Devices.-.HelloToast.2026-04-09.22-02-37.zip)

---

## Fonctionnalités

- **Bouton "Afficher un message"** → affiche un Toast "Bonjour !" en bas de l'écran
- **Bouton "Incrémenter le compteur"** → ajoute 1 au compteur affiché dans un cadre

---

## Structure du projet

```
app/
├── src/main/
│   ├── java/.../MainActivity.java       # Logique de l'application
│   └── res/
│       ├── layout/activity_main.xml     # Interface utilisateur
│       ├── drawable/border_box.xml      # Cadre rouge du compteur
│       └── values/themes.xml           # Thème de l'application
```

---

## Fichiers modifiés

### `activity_main.xml`
Définit l'interface avec :
- Un fond noir (`background="#000000"`)
- Un compteur entouré d'un cadre rouge carmin (`@drawable/border_box`)
- Deux boutons en rouge carmin (`backgroundTint="#DC143C"`)

### `border_box.xml`
Fichier drawable qui dessine le cadre autour du compteur :
- Bordure rouge carmin (`#DC143C`) de 2dp
- Coins arrondis de 12dp
- Fond noir

### `themes.xml`
Force le fond de la fenêtre entière en noir via :
```xml
<item name="android:windowBackground">#000000</item>
```

### `MainActivity.java`
Contient la logique :
- `Toast.makeText(...).show()` → affiche le message temporaire
- `count++` + `setText()` → incrémente et met à jour l'affichage

---

## Lancer le projet

1. Clone le repo :
```bash
git clone https://github.com/TON_USERNAME/TON_REPO.git
```
2. Ouvre le projet dans **Android Studio**
3. Lance un émulateur ou connecte un appareil Android
4. Clique sur Run

---

## Prérequis

- Android Studio Hedgehog ou plus récent
- SDK Android API 24 minimum
- Java 11+

---

## Concepts abordés

| Concept | Description |
|---|---|
| `Toast` | Message temporaire affiché à l'écran |
| `Button.setOnClickListener` | Gestion des clics sur un bouton |
| `TextView.setText()` | Mise à jour dynamique du texte |
| `drawable` XML | Création de formes personnalisées |
| `themes.xml` | Personnalisation du thème global |

---

## Auteur

Réalisé dans le cadre d'un TP de développement Android mobile.
