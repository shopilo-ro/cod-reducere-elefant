# Cod reducere Elefant — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Elefant** de pe [shopilo.ro](https://shopilo.ro/magazin/elefant.ro). Returneaza **cupoane Elefant** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-elefant](https://shopilo-ro.github.io/cod-reducere-elefant/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-elefant
cd cod-reducere-elefant
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Elefant",
    "code": "SHOPILO20",
    "discount": "20 lei",
    "description": "20 lei reducere la orice produs",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/elefant.ro"
  }
]
```

## Cupoane Elefant disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20 lei | 20 lei reducere la orice produs | [shopilo.ro](https://shopilo.ro/magazin/elefant.ro) |

Codurile active: **[shopilo.ro/magazin/elefant.ro](https://shopilo.ro/magazin/elefant.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Elefant?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/elefant.ro), adauga produsele in cos pe Elefant, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Elefant?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Elefant?
Pagina [shopilo.ro/magazin/elefant.ro](https://shopilo.ro/magazin/elefant.ro) este actualizata zilnic cu cele mai noi cod reducere Elefant, voucher Elefant si cupon promotional Elefant.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Elefant

Elefant este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/elefant.ro) cele mai bune cod reducere Elefant, cupoane Elefant verificate si voucher Elefant active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-elefant
```

```javascript
const { fetchCoupons } = require('cod-reducere-elefant');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
