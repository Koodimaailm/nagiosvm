# Ruuter RB1100ahx4 A Käsud

## ALGUS KÄSUD

``
en - annab privileegid seadistusele
``

``
conf t - ligipääs seadistamisele
``

## PESA 1 SEADISTAMISE KÄSUD

``
int fa0/1 - valib pesade asukoha näiteks pesa  1 või 2 reast 1
``

``
ip address 10.10.15.25 255.255.255.0 - määrab interneti protokolli aadressi ja võrk sees võrgus ehk (Subneti)
``

``
no shutdown - käsib sellel pesal automaatselt käivitada süsteemi alg käivitamisel Eelnevad tähendused on seotud VOIP ehk Internetitelefonide ülesseseadistamisega kus tegemist on siis ruuteri häälestamisega.
``


## DHCP seadistamine ruuteris 
``
ip dhcp pool VOICE - määrad DHCP ehk (Dynamic Host Configuration Protocol) häälestusele spetsiaalse nime interneti protokollile mis võib olla ka erineva nimega.
``

``
network 10.10.15.0 255.255.255.0 - määrab kindla ulatuse addresside jagamisel nagu DHCP lubab
``

``
default-router 10.10.15.25 - - peamise andmeedastus või võrgu ruuteri aadressi määramine.
``

``
option 150 ip 10.10.15.25 - määrab TFTP ehk (Trivial File Transfer protocol) aadressi.
``



## Telefoni teenuse seadistus 

``
telephony-service - annab loa siseneda telefoni teenuse valikutesse
``

``
max-dn 5 - määrab maksimaalse kõneliini koguse.
``

``
max-ephones 5 - määrab maksimaalse kõneliini seadmete koguse.
``

``
auto assign 4 to 6 - määrab addresside vahemiku.
``

## Telefoni seadistus ruuteris

``
ephone-dn 1 - valib ühendatud seadme milleks on seade 1.
``

``
number 112 - käsk mis määrab VOIP telefonidele kõne numbri
``


# Võrgulüliti A käsud SGS-6341-24P4X


##  VLAN seadistus 

``
int range fa0/1 - 5 - valib määratud vahemikus kaabli pesasi.
``

``
switchport mode access -  määrab kaabli liidese oleku käsku.
``

``
switchport voice vlan 1 - suunab kõne kanali teenuse kasutatavasse pessa 1.
``

[Käskude andmebaas](https://notes.networklessons.com/)




 








 
