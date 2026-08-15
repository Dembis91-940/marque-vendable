# Marque Vendable — Playbook « Construire une marque vendable »

> **Thorne vendue 3,8 Md$ à P&G. Béis valorisée 210 M$.** Deux marques solo, une méthode : le playbook pour construire une marque qu'on vous achète.

**Live :** https://dembis91-940.github.io/marque-vendable/ (GitHub Pages)

## Business model

| Élément | Détail |
|---|---|
| **Cible** | Fondateurs et dirigeants de PME/startups qui veulent construire une marque valorisable (exit, levée, transmission) |
| **Problème** | La plupart des marques ne sont pas vendables : pas de positionnement premium, pas de preuve documentée, pas de metrics build-to-sell, due diligence impossible |
| **Solution** | Playbook 60-80 pages (2 études de cas décortiquées : Thorne, Béis) + 5 templates prêts à remplir + pack avec audit manuel |
| **Prix** | Playbook PDF 19 € · Playbook + 5 templates 39 € · Pack préparation à l'exit (avec audit) 79 € |
| **Marge** | ~98 % (produit digital, livraison email automatisée) |
| **Canal** | LinkedIn (fondateurs, M&A), newsletter, SEO « marque vendable », bouche-à-oreille |

## Pages

| Fichier | Rôle |
|---|---|
| `index.html` | Landing immersive 3D (Three.js, parallaxe, particules cyan/violet) : hero Thorne/Béis, stats, 8 chapitres, 3 offres, tunnel de commande EmailJS, garantie 14 jours |
| `vente.html` | Page de vente dédiée : 3 offres, tunnel EmailJS, garantie, 3D |
| `playbook-marque-vendable.md` | Le playbook complet (source) |
| `PDF/playbook-marque-vendable.pdf` | Le playbook en PDF, prêt à livrer |
| `templates/` | 5 templates remplissables : positionnement, metrics tracker, fiche due diligence, chronologie d'exit, pitch d'acheteur |
| `emails/` | Séquence email de 3 messages : valeur, templates en action, objection prix |
| `chatbot-config.js` + `chatbot.js` | Chatbot FAQ + capture de leads (EmailJS) |
| `assets/js/voice-config.js` + `voice-widget.js` | Widget vocal intégré (en pause faute de crédits Vapi — à activer en remplissant `assistantId`) |

## Zéro simulateur — preuves

Le tunnel de commande envoie de **vrais emails** via EmailJS (service `service_cy1ytdb`, template `template_xpo58cv`) : chaque commande arrive dans la boîte mail d'El mouskito, qui livre le playbook PDF sous 24-48 h (pack exit : audit manuel planifié sous 72 h).

## Déploiement

```bash
cd ~/Documents/livrables/marque-vendable
git add -A && git commit -m "Mise à jour"
git push origin main
```

Pages activées sur le dépôt GitHub `Dembis91-940/marque-vendable` (branch `main`, dossier racine).

## Ce qui reste

- Stripe (paiement en ligne automatisé) : en attente chez l'utilisateur — en attendant, paiement par virement ou message direct, documenté dans l'email de confirmation.
- Widget vocal : activer en renseignant `publicKey` + `assistantId` Vapi dans `assets/js/voice-config.js` (crédits en pause).
