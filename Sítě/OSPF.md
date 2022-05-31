# OSPF vs RIP

- Nelimituje hop count
- Používá VLSM
- Obnovení posílá multicastem
- Obnovení posílá jen při změně
- Rozděluje síť na oblasti
- Povoluje authentifikaci
- Sousední routery si mezi sebou posílají link-state updates
- LSDB (Link-state database)
- Sousedská tabůlka
- Topologická tabůlka
  - Nejlepší alternativní cesty
- Routovací tabůlka
  - Momentální nejlepší cesty
### Oblasti
- Hlavní oblast 0
### Link State Advertisement (LSA)
- 11 typů LSA packetů
- Informace o topologii
### Link State Database (LSDB)
### Link State Request (LSR)
- Žádá sousední routery o informace, které chybí v LSDB
### Link State Update (LSU)
- Odpovídají na LSR, s částí databáze
### Link State Acknowledgement (LSAck)
- Podtvrzuje LSU packet
#### Routery v oblasti se zařazují do dvou skupin:
- Area Border Router (ABR)
  - Propojuje oblasti
- Autonomous System Boundary Router (ASBR)
  - Propojuje routery s ostatními routovacími protokoly
- Designated Router (DR)
  - Zvolen ostatními routery v oblasti podle priority
- Backup Designated Router (BDR)
  - Stává se DR routerem, když DR router selže
<b> Každý router má ID ve formátu IPv4 adresy </b> 

<b> Priorita volby DR </b> 

- Manuálně nastavená priorita
- Největší router ID
- Největší nastavená IP adresa
- Největší loopback adresa
- Nastavení ospf na routeru

> Router(config)# router ospf process ID

> Router(config)# router-id x.x.x.x

> Router(config-router)# network ip address wildcard mask area area id
