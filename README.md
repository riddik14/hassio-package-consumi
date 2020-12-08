# hassio-package-consumi

package consumi
<img src="https://github.com/riddik14/hassio-package-consumi/blob/main/image_.png">

- il progetto parte lavoro di Mauro Cimino che approfitto per ringraziarlo ed è esteso al calcolo tariffe
- contatti: 'riddik14 - github- telegram @riddik14'

- https://hassiohelp.eu/2019/03/02/controllo-consumi-costi/

- https://hassiohelp.eu/author/legolas08/


- Implementazione della fascia F3 e calcolo bolletta su giorno mensile e annuale, hai bisogno di un sensore 
- che indichi il consumo in kWh da inserire nella prima parte del package - esempio di sensori compatibili 
- pzem - shellyPm - shellyem e altri compatibili con hassio
-
-
- INSTALLAZIONE

- 1. copiare il file pkg_tariffe_luce_consumi.yaml nella cartella "/config/packages" e aggiungere alla riga 19 il tuo sensore watt
- se usi shelly ti consiglio di far passare il sensore che ti indica i watt attraverso il convertitore kwh, qui un esempio
<xmp>
   ...code...
    ##--------------------- IMPOSTAZIONI DEL PACKAGE ---------------------##
      setting:

        Sensore: &sensore_misura_energia sensor.energia_kwh
        #nel caso di utilizzo di convertitore inserire su sensor.energia_kwh e qui sotto
        # il sensore kw. nel caso si vuole la conversione inserire il sensore dopo &sensore_misura_energia2 qui sotto 
        Sensore_wh_to_kwh: &sensore_misura_energia2 sensor.ripostiglio_energy_power
        TariffaF1: &tariffaf1 0.0869847
        TariffaF2: &tariffaf2 0.0869847
        TariffaF3: &tariffaf3 0.0869847
        Accisa: &accisa 0.0227           #calcolo medio sulla bolletta
        Iva: &iva 10                     #IVA
        trasporto: &trasporto 0.07224    #calcolo medio sulla bolletta
        
    ##--------------------- IMPOSTAZIONI DEL PACKAGE ---------------------##  
- 2. installare dal menu frontend di hacs i seguenti:

- vertical-stack-in-card
- mini-graph-card
- banner-card
- paper-buttons-row
- state-switch

- aprire il file  lovelace-dash.txt e 
- copiare il contenuto in una card manuale dalla dashbord del tuo assistente
-  alla riga 8 della card mettere il sensore volt
-  alla riga 31 il proprio sensore watt
-  infine salvare la card


- per chi ha pannelli solari posso suggerire questa repository https://github.com/riddik14/tesla-style-solar-power-card

<img src="https://github.com/reptilex/tesla-style-solar-power-card/raw/master/tesla-style-card-animation.gif">


<a href="https://www.buymeacoffee.com/T1Pqksy" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/arial-black.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>


- Se il progetto ti è piaciuto clicca <a href="https://www.paypal.me/DomenicoCeccarelli">qui</a> per offrirmi un caffè

