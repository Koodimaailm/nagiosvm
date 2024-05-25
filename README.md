# Ruuter A Käsud 2811(Ruuter)

## ALGUS KÄSUD

``
en - annab privileegid seadistusele
``

``
conf t - ligipääs seadistamisele
``

## PESA 1 SEADISTAMISE KÄSUD

``
int fa0/1 - valib pesa 0 reast 1
``

``
ip address 10.10.15.25 255.255.255.0 - määrab interneti protokolli aadressi ja subneti
``

``
no shutdown - käsib sellel pesal automaatselt käivitada
``


## DHCP seadistamine ruuteris 
``
ip dhcp pool VOICE - määrad dhcp häälestuse nime
``

``
network 10.10.15.0 255.255.255.0 - määrab ulatuse addresside andmisel'
``

``
default-router 10.10.15.25 - peamise ruuteri aadressi määramine
``

``
option 150 ip 10.10.15.25 - määrab TFTP aadressi
``



## Telefoni teenuse seadistus 

``
telephony-service - annab loa seadistada telefoni teenust
``

``
max-dn 5 - määrab maksimaalse kõneliini koguse
``

``
max-ephones 5 - määrab maksimaalse seadme koguse
``

``
auto assign 4 to 6 - vormistab addresse vahemikus
``

## Telefoni seadistus ruuteris

``
ephone-dn 1 - valib ühendatud seadme milleks on seade 1
``

``
number 112 - määrab sellele VoIP seadmele kõne numbri
``


# Lüliti A käsud 24TT või muu (Ruuter)


##  VLAN seadistus

``
int range fa0/1 - 5 - krabab määratud vahemikus pesasi
``

``
switchport mode access - määrab liidese käsku
``

``
switchport voice vlan 1 - suunab kõnekanalit LAN 1.
``






 








 