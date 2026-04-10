# Codice sconto Booking.com, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Booking.com** da [shopilo.it](https://shopilo.it/negozi/booking.com). Restituisce **coupon Booking.com** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-booking](https://shopilo-it.github.io/codice-sconto-booking/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-booking
cd codice-sconto-booking
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Booking.com",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su hotel e alloggi",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/booking.com"
  }
]
```

## Coupon Booking.com disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su hotel e alloggi | [shopilo.it](https://shopilo.it/negozi/booking.com) |

Codici attivi: **[shopilo.it/negozi/booking.com](https://shopilo.it/negozi/booking.com)**

## Domande frequenti

### Come utilizzo un codice sconto Booking.com?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/booking.com), aggiungi i prodotti al carrello su Booking.com e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Booking.com?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Booking.com piu recenti?
La pagina [shopilo.it/negozi/booking.com](https://shopilo.it/negozi/booking.com) viene aggiornata quotidianamente con i codici sconto Booking.com, voucher Booking.com e coupon promozionali Booking.com piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Booking.com

Booking.com e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/booking.com) trovi i migliori codici sconto Booking.com, coupon Booking.com verificati e voucher Booking.com attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-booking
```

```javascript
const { fetchCoupons } = require('codice-sconto-booking');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
