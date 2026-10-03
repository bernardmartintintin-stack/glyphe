# Glyphe

Dessinez directement sur votre écran avec un simple raccourci clavier. Une barre d'outils flottante apparaît en haut de l'écran, vos annotations restent affichées par-dessus vos applications.

## Installation

### Linux

```bash
curl -fsSL https://raw.githubusercontent.com/TON_PSEUDO/glyphe/main/install.sh | bash
```

### Windows (PowerShell)

```powershell
irm https://raw.githubusercontent.com/TON_PSEUDO/glyphe/main/install.ps1 | iex
```

Les installeurs mettent en place Node.js si nécessaire, installent Glyphe, créent un raccourci et lancent le programme.

### Depuis les sources

```bash
git clone https://github.com/TON_PSEUDO/glyphe.git
cd glyphe
npm install
npm start
```

Ou lancez directement l'installeur local : `bash install.sh` (Linux) ou `powershell -ExecutionPolicy Bypass -File .\install.ps1` (Windows).

## Utilisation

| Raccourci | Action |
| --- | --- |
| Ctrl + Alt + D | Activer / désactiver le mode dessin |
| Ctrl + Alt + Q | Quitter |
| Ctrl + Z / Ctrl + Y | Annuler / rétablir |
| Échap | Masquer la barre (les dessins restent) |

Les raccourcis, les couleurs, le thème et l'orientation de la barre se changent dans les paramètres.

## Mode essentiel

Au début de `index.html`, `const ESSENTIAL=true;` limite l'application à l'essentiel. Passez la valeur à `false` pour activer tous les outils (laser, formes, texte, projecteur, capture d'écran, etc.).

## Désinstallation

Linux : `bash install.sh --uninstall`

Windows : `powershell -ExecutionPolicy Bypass -File .\install.ps1 -Uninstall`

## Licence

MIT
