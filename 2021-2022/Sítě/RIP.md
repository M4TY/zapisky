# RIP
- Routing Information Protocol
- Používá k výměně informací UDP packety
- Routovací informace se zasílají kazdých 30s (advertising) nebo při změně topologie
- Timeout 240s => packet je odebrán z routovacích tabůlek
- nepoužívá se, RIPv2
- Je založený na vzdálenosti vektorové strategii
- Cena metriky je počet hopů k destinaci
    - Není ideální řešení
- Nekonečno definováno jako 16 => vhodný pro malé sítě


## Nevýhody RIP
- HOP count není ideální metrika
- Nepodporuje VLSM, je classfull routing protocol
- Broadcastuje routovací tabulku do celé sítě
    - Zahlcování sítě
- Pomalá konvergence - při selhání trvá minutu stabilizovat novou cestu
- Maximální vzdálenost 15 hopů
- Není spolehliv

## Výhody RIP
- Nenáročný na nastavení

## Konfigurace
- Povolení RIP protokolu


```
(config)# router rip


```
- Zapnutí verze 2 RIP


```
(config-router)# version 2

```

```
(config-router)# no auto-summary
```

- Určení sítí, které má RIP spravovat (maska není potřeba)


```
(config-router)# network X.X.X.X
```

Nastavení propagace default gatewaye 

```
(config-router)# default-information originate
```
