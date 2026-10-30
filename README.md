# Cartes de visite Stela

Fiches contact à la charte Stela, une par personne, accessibles par QR code ou NFC.

- Fiches : `https://avistar-info.github.io/stela-cartes/<prenom>/`
- QR codes prêts à imprimer : dossier `qr/` (PNG haute définition + SVG)

## NFC

Écrire sur la puce un enregistrement **URL** avec le lien de la fiche, par exemple avec l'app NFC Tools. Ne pas y écrire de vCard : le lien permet de modifier la fiche sans toucher à la puce.

## Modifier une info

1. Modifier `contacts.json`.
2. `pip install segno` puis `python3 build.py`
3. Commit + push : le site se met à jour en ~1 min. **Les QR codes et les puces NFC ne changent pas.**
