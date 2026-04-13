# Code promo Cdiscount, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Cdiscount** depuis [shopilo.fr](https://shopilo.fr/reductions/cdiscount.com). Renvoie les **coupons Cdiscount** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-cdiscount](https://shopilo-fr.github.io/code-promo-cdiscount/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-cdiscount
cd code-promo-cdiscount
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Cdiscount",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur l'electronique et la maison",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/cdiscount.com"
  }
]
```

## Coupons Cdiscount disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur l'electronique et la maison | [shopilo.fr](https://shopilo.fr/reductions/cdiscount.com) |

Codes actifs : **[shopilo.fr/reductions/cdiscount.com](https://shopilo.fr/reductions/cdiscount.com)**

## Questions frequentes

### Comment utiliser un code promo Cdiscount ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/cdiscount.com), ajoutez les produits a votre panier sur Cdiscount et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Cdiscount ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Cdiscount les plus recents ?
La page [shopilo.fr/reductions/cdiscount.com](https://shopilo.fr/reductions/cdiscount.com) est mise a jour quotidiennement avec les codes promo Cdiscount, bons de reduction Cdiscount et coupons promotionnels Cdiscount les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Cdiscount

Cdiscount est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/cdiscount.com), retrouvez les meilleurs codes promo Cdiscount, coupons Cdiscount verifies et bons de reduction Cdiscount actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-cdiscount
```

```javascript
const { fetchCoupons } = require('code-promo-cdiscount');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
