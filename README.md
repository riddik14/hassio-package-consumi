### homeassistant-package-consumi ###
<img src="https://github.com/riddik14/hassio-package-consumi/blob/main/output_DrKr3V.gif"> | 
<img src="https://github.com/riddik14/hassio-package-consumi/blob/main/image_.png">

---------------------------
**Contributi:**
Il progetto è parte lavoro di Mauro Cimino che approfitto per ringraziarlo ed è esteso al calcolo tariffe.
Roberto Piumatti lo ha adeguato a quanto stabilisce la legge sul calcolo della bolletta. 
contatti: 'riddik14 - github - chat telegram https://t.me/joinchat/Fanqz1jiL42Y0Hzd - e - robertopiumatti - github'

- https://hassiohelp.eu/2019/03/02/controllo-consumi-costi/
- https://hassiohelp.eu/author/legolas08/


--------------------------
**Sensori compatibili:**
- pzem 
- shellyPm 
- shellyem
- clamp su esp8266 pin A0 con esphome firmware https://esphome.io/components/sensor/pzem004t.html?highlight=pzem#see-also
- altri (suggeritemi altri)


**INSTALLAZIONE**

1. copiare il file pkg_consumi.yaml e secrets.yaml (se gia esistente copiare l contenuto del vostro sectrets.yaml) nella cartella "/config/packages" e modificarlo seguendo le istruzioni interne al file secrets.yaml.

2. installare dal menu frontend di hacs i seguenti:

- vertical-stack-in-card

- mini-graph-card

- banner-card

- paper-buttons-row

- state-switch

- bar-card



aprire il file  lovelace-dash.txt o lovelace-dash-light.txt e copiarne il contenuto in una card manuale dalla dashbord del tuo assistente.
Alla riga 8 della card mettere il sensore volt alla riga 32 il proprio sensore watt, infine salvare la card.

____________________________________

in aggiunta suggerisco il seguente pacchetto di hassio help sempre di Mauro Cimino 
_______________
<img src="https://hassiohelp.eu/wp-content/uploads/2020/10/new-controllo-carichi_00.jpg">
_______________
https://hassiohelp.eu/2020/10/14/nuovo-controllo-carichi/


====================================

Per chi ha pannelli solari posso suggerire questa repository https://github.com/riddik14/tesla-style-solar-power-card


<img src="https://github.com/reptilex/tesla-style-solar-power-card/raw/master/tesla-style-card-animation.gif">
____________________________________

<a href="https://www.buymeacoffee.com/T1Pqksy" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/arial-black.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>

------------------------------------


Se il progetto ti è piaciuto clicca <a href="https://www.paypal.me/DomenicoCeccarelli">qui</a> per offrirmi un caffè

