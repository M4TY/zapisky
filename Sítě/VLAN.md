# VLAN

## Výhody VLAN
- Bezpečnost
- Snížení ceny
- Lepší výkon

### Commandy

#### Zobrazení VLANů
- `# show vlan brief`

#### Tvorba VLAN
- `# conf t`
- `(config)# vlan <number>`
- `(config)# name <vlan_name>`
- `(config)# end`
- **Číslovat VLAN podle subnety**
- př.: `172.17.10.21 -> VLAN 10`

#### Přiřazení portů
- `# conf t`
- `(config)# interface <port>`
- `(config-if)# switchport mode access`
- `(config-if)# switchport access vlan <cislo>`
- `(confif-if)# end`

#### Tvorba Trunku
- `# conf t`
- `(config)# interface <port>`
- `(config-if)# switchport mode trunk`
- `(config-if)# switchport trunk native vlan <cislo>`
- `(config-if)# switchport trunk allowed vlan <cislo>,<cislo>,<cislo>,<cislo>...`
- `(config-if)# end`
- **Nepovolovat víc VLANů než je potřeba**

#### Mazání VLANů
- `# no vlan <cislo>`
- **Smazáním VLANy by se měly přiřadit všechny porty do jiné VLANy**
- Smazat celý vlan.dat lze pomocí `delete flash:vlan.dat`

#### Kontrola VLAN
- `# show id <cislo>`
    - Zobrazení vlan id podle čísla vlan
- `# show vlan summary`
- `# show interfaces <port> switchport`
    - Zobrazení nastavení portu

### Typy VLAN
#### Defaultní VLAN
- VLAN 1 na cisco switchi
- 1002-1005 pro zastaralé technologie
#### Data VLAN
- Určená pro komunikaci mezi zařízeníma (2-1001)
#### Management VLAN
- Používá se na síťový management provozu jako SSH, Telnet, HTTPS, HTTP a SNMP
#### Voice VLAN
- Voice over IP (VoIP)
#### Native VLAN
- Každé zařízení musí patřit do nějaké VLAN, při segmentování sítě
- Best practise je nakonfigurovat VLAN jako VLAN, která se jinde v síti nepoužívá, např.: VLAN 99

#### VLAN Trunk
- Trunk nepatří do žádné VLAN
- Přes trunk porty můžou chodit data z více VLAN

#### VLAN Access
- Access port pouze pro jednu VLAN

#### VLAN Tag políčka
- **IEEE 802.1Q Tagging**
- **Typ**
- **Pri**
- **CFI**
- **VID**
    - VLAN ID
    - Označí VLAN

#### VLAN Rozsahy
- **Normal range**
    - 1-1005
- **Extended range**
    - 1006-4094

### Dynamic Trunking Protocol
