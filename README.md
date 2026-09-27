# AION 2 Discord Rich Presence for Windows 10/11

**English** · [Français](#français)

Show your **AION 2** session on Discord with a dedicated Windows app. It starts quietly with the game, uses the game's session time, and closes when the game exits. Game process detection supports **Global, Taiwan (TW), and Korea (KR)** clients. Automatic character name detection from the game window title has been verified on TW.

## Download and install

1. Download [AionPresence-Setup-0.7.0.exe](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.0/AionPresence-Setup-0.7.0.exe).
2. Run the installer on Windows 10 or 11. Open **AION 2 Discord Presence** from the Start menu once to set up automatic launch.
3. Keep the Discord desktop app open. A shared Discord Application ID and presence artwork are configured by default. Choose your language and visibility settings in the app.

Installation is required; no PowerShell window opens. The installer is currently **unsigned**, so Windows may display a warning. You can verify the download with its [SHA-256 checksum](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.0/AionPresence-Setup-0.7.0.sha256).

## Screenshots

![AION 2 Discord Presence overview](images/overview-en.png)

![AION 2 Discord Presence settings](images/settings-en.png)

![Update settings with automatic updates off by default](images/updates-en.png)

![Visibility settings, including the GitHub button](images/visibility-en.png)

## Features

- Automatic launch to the notification area with `Aion2.exe`, and automatic exit when the game closes.
- Character name from the game window title when available, with a manual fallback.
- Timer based on the game process start time, preserved when the presence app restarts.
- French or English interface and presence, with individual visibility controls.
- Global EU, NA, SA and JP server regions, plus TW and KR client detection.
- Game image and class icons, including Brawler, in the Discord presence.
- A Discord button linking to this project's latest GitHub download page. Enabled by default; switch it off in Settings → Visibility.
- Check and install updates in the app. Automatic installation is available in Settings → Updates and is off by default. Downloaded installers are checked against GitHub's SHA-256 digest.
- Local preview, saved preferences, and configurable close button behavior.

Level, zone, and party are not yet read directly from the game. They appear only when a compatible profile data source supplies them. Automatic server and class detection also depends on such a source; manual fallbacks are available.

## FAQ

**Do I need to create a Discord application?** No. A shared Application ID is included. You can enter your own ID in Settings if you prefer.

**Does the app need to stay open?** It can remain in the notification area. After its first launch, a lightweight watcher starts with Windows and opens the presence app only when the game starts.

**Why can't I see the GitHub button on my own Discord presence?** [Discord shows Rich Presence buttons only to other users](https://docs.discord.com/developers/discord-social-sdk/development-guides/setting-rich-presence#setting-buttons). Ask a friend or use a second account to view your profile and check the button.

**How do updates work?** Use Settings → Updates to check and install. When automatic updates are enabled, the app checks at most every six hours and installs a newer release if available. The app briefly closes while the installer replaces it, then restarts. Version 0.6.1 must be upgraded to 0.7.0 with the installer once; in-app updates work from 0.7.0 onward.

**How do I uninstall it?** Use **Windows Settings → Installed apps → AION 2 Discord Presence**.

**How can I report a problem?** Open an [issue](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/issues) with your Windows version, game client region, and a description. Please do not attach personal data.

---

## Français

Affichez votre session **AION 2** sur Discord avec une application Windows dédiée. La présence démarre discrètement avec le jeu, utilise son temps de session et disparaît quand vous le quittez. La détection du processus prend en charge les clients **Global, Taïwan (TW) et Corée (KR)**. La lecture automatique du nom du personnage dans le titre de la fenêtre a été vérifiée sur TW.

### Télécharger et installer

1. Téléchargez [AionPresence-Setup-0.7.0.exe](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.0/AionPresence-Setup-0.7.0.exe).
2. Lancez l'installateur sur Windows 10 ou 11, puis ouvrez une fois **AION 2 Discord Presence** depuis le menu Démarrer pour activer le lancement automatique.
3. Gardez l'application Discord de bureau ouverte. L'Application ID partagé et les images de la présence sont déjà configurés. Choisissez la langue et les informations affichées dans les paramètres.

L'installation est requise et aucune fenêtre PowerShell ne s'ouvre. L'installateur est actuellement **non signé** ; Windows peut afficher un avertissement. Vérifiez le fichier téléchargé avec sa [somme SHA-256](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.0/AionPresence-Setup-0.7.0.sha256).

### Captures d'écran

![Vue d'ensemble de l'application](images/overview-fr.png)

![Paramètres de l'application](images/settings-fr.png)

![Paramètres des mises à jour automatiques désactivées par défaut](images/updates-fr.png)

![Options de visibilité avec le bouton GitHub](images/visibility-fr.png)

### Fonctions

- Démarrage automatique et discret dans la zone de notification avec `Aion2.exe` ; arrêt à la fermeture du jeu.
- Nom du personnage lu dans le titre de la fenêtre du jeu lorsque le client le fournit, avec un champ de secours.
- Chrono fondé sur l'heure de démarrage du jeu, conservé si l'application de présence redémarre.
- Interface et présence en français ou en anglais, avec choix individuel des informations affichées.
- Régions Global EU, NA, SA et JP, ainsi que détection des clients TW et KR.
- Image du jeu et icônes des classes, dont Brawler, dans la présence Discord.
- Bouton Discord vers la page GitHub de la dernière version. Il est activé par défaut et désactivable dans **Paramètres → Visibilité**.
- Recherche et installation des mises à jour depuis l'application. L'installation automatique est disponible dans **Paramètres → Mises à jour** et désactivée par défaut. L'installateur téléchargé est vérifié avec l'empreinte SHA-256 fournie par GitHub.
- Aperçu local, préférences sauvegardées et comportement du bouton de fermeture au choix.

Le niveau, la zone et le groupe ne sont pas encore lus directement dans le jeu. Ils s'affichent seulement si une source de profil compatible les fournit. La détection automatique du serveur et de la classe dépend aussi d'une telle source ; des champs de secours sont disponibles.

### Questions courantes

**Faut-il créer une application Discord ?** Non. Un Application ID partagé est intégré. Vous pouvez saisir le vôtre dans les paramètres.

**L'application doit-elle rester ouverte ?** Elle peut rester dans la zone de notification. Après sa première ouverture, un surveillant léger démarre avec Windows et ouvre l'application seulement lorsque le jeu se lance.

**Pourquoi le bouton GitHub n'apparaît-il pas sur ma propre présence Discord ?** [Discord affiche les boutons Rich Presence uniquement aux autres utilisateurs](https://docs.discord.com/developers/discord-social-sdk/development-guides/setting-rich-presence#setting-buttons). Demandez à un ami ou utilisez un second compte pour vérifier le bouton sur votre profil.

**Comment se font les mises à jour ?** Utilisez **Paramètres → Mises à jour** pour rechercher et installer. Si l'option automatique est activée, l'application vérifie au plus toutes les six heures et installe une nouvelle version disponible. Elle se ferme brièvement pendant l'installation, puis redémarre. La version 0.6.1 doit être remplacée une fois avec l'installateur 0.7.0 ; les mises à jour intégrées fonctionnent à partir de 0.7.0.

**Comment la désinstaller ?** Dans **Paramètres Windows → Applications installées → AION 2 Discord Presence**.

**Où signaler un problème ?** Ouvrez une [issue](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/issues) avec la version de Windows, la région du client et une description du problème, sans données personnelles.

---

Unofficial fan application / Application de fans non officielle. Not affiliated with NCSOFT or Discord / Sans affiliation avec NCSOFT ou Discord. © 2026 KaiiZzeR971. [License notice](LICENSE.txt).
