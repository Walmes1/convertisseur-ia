# 🪶 Convertisseur Fichiers → IA

Page web **100% navigateur** (aucun serveur, rien n'est envoyé sur internet) qui convertit
tes documents au format le plus **léger et lisible pour une IA** comme Claude : le **Markdown** (`.md`).

## Utilisation
1. Ouvre `index.html` (double-clic) — ou héberge le dossier sur n'importe quel hébergeur statique gratuit (Netlify, GitHub Pages, Vercel…).
2. Dépose tes fichiers à **gauche**.
3. Récupère les versions converties à **droite**, même nom au format `.md`.
   - Bouton 👁 = aperçu, ⬇ = télécharger un fichier, **Tout télécharger (.zip)** pour tout d'un coup.

## Formats gérés
| Entrée | Conversion |
|---|---|
| **PDF** (texte) | texte extrait page par page |
| **Word** `.docx` | Markdown (titres, listes, gras…) |
| **Excel** `.xlsx/.xls` | tableaux Markdown (1 par feuille) |
| **CSV** | tableau Markdown |
| **PowerPoint** `.pptx` | texte par diapositive |
| **HTML** | Markdown propre |
| **JSON** | bloc de code formaté |
| **RTF** | texte nettoyé |
| **TXT / MD** | repris tel quel |

> ⚠️ Les PDF **scannés** (image) n'ont pas de texte extractible — un message le signale.
> Pour ceux-là, mieux vaut donner l'image directement à l'IA (Claude lit les images nativement).

## Pourquoi le Markdown ?
Une IA facture et lit en **tokens** (≈ 4 caractères = 1 token). Le Markdown supprime tout le
poids inutile d'un PDF/DOCX et garde juste le texte structuré → **moins cher, plus rapide, plus fiable**.

## Technique
Tout est dans `index.html`. Conversions côté client via : pdf.js, mammoth.js, SheetJS, JSZip, Turndown (chargés en CDN).

## Essayer en ligne / Try it online
👉 **https://walmes1.github.io/convertisseur-ia/** — gratuit, sans pub, sans inscription. Free, no ads, no sign-up.

## Télécharger / Download
[⬇ Dernière version (.zip)](https://github.com/Walmes1/convertisseur-ia/releases/latest) — dézipper puis ouvrir `index.html`.

## Licence
MIT — © Messaoudi Oualid. Libraries: pdf.js (Apache-2.0), mammoth.js (BSD-2), SheetJS (Apache-2.0), JSZip (MIT), Turndown (MIT).
