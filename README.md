# Cod reducere OVS — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere OVS** de pe [shopilo.it](https://shopilo.it/magazin/ovs.it). Returneaza **cupoane OVS** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-ovs](https://shopilo-it.github.io/codice-sconto-ovs/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-ovs
cd codice-sconto-ovs
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "OVS",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su abbigliamento uomo e donna",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/ovs.it"
  }
]
```

## Cupoane OVS disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% di sconto su abbigliamento uomo e donna | [shopilo.it](https://shopilo.it/magazin/ovs.it) |

Codurile active: **[shopilo.it/magazin/ovs.it](https://shopilo.it/magazin/ovs.it)**

## Intrebari frecvente

### Cum folosesc un cod de reducere OVS?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/ovs.it), adauga produsele in cos pe OVS, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele OVS?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri OVS?
Pagina [shopilo.it/magazin/ovs.it](https://shopilo.it/magazin/ovs.it) este actualizata zilnic cu cele mai noi cod reducere OVS, voucher OVS si cupon promotional OVS.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre OVS

OVS este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/ovs.it) cele mai bune cod reducere OVS, cupoane OVS verificate si voucher OVS active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-ovs
```

```javascript
const { fetchCoupons } = require('codice-sconto-ovs');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
