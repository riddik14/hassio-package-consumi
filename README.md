# hassio-package-consumi

package consumi
<img src="https://github.com/riddik14/hassio-package-consumi/blob/main/image_.png">

- il progetto parte lavoro di Mauro Cimino che approfitto per ringraziarlo ed è esteso al calcolo tariffe
- contatti: 'riddik14 - github- telegram @riddik14' - e - robertopiumatti - github 

- https://hassiohelp.eu/2019/03/02/controllo-consumi-costi/

- https://hassiohelp.eu/author/legolas08/


- Implementazione della fascia F3 e calcolo bolletta su giorno mensile e annuale, hai bisogno di un sensore 
- che indichi il consumo in kWh da inserire nella prima parte del package - esempio di sensori compatibili 
- pzem - shellyPm - shellyem e altri compatibili con hassio
-
-
- INSTALLAZIONE

- 1. copiare il file pkg_tariffe_luce_consumi.yaml nella cartella "/config/packages" e aggiungere alla riga 29 il tuo sensore watt
- se usi shelly ti consiglio di far passare il sensore che ti indica i watt attraverso il convertitore kwh, qui un esempio di come 
- è settata la riga 29 e alla riga 38 il sensore shelly
<xmp>
   
  ##--------------------- IMPOSTAZIONI DEL PACKAGE ---------------------##
  setting:

    # nel caso si disponga di un sensore di energia (kWh) inserirlo qua
    Sensore: &sensore_misura_energia sensor.pzem_energy_today #sensor.energia_kwh

    # SOLO NEL CASO NON SI DISPONGA DI UN SENSORE DI ENERGIA, ma solo del sensore di potenza instantanea:
    # 1. decommentare le riga sotto (riga 29)
    # 2. inserire il nome del sensore di potenza instantanea (W)
    # 3. decommentare sensore di integrazione (riga 84-88)
    # 4. inserire il nome del sensore di integrazione sensor.energia_kwh nel sensore di energia sopra (riga 21)

    #Sensore_w_to_kwh: &sensore_misura_energia2 sensor.ripostiglio_energy_power
    
    # Materia Energia
    MateriaEnergiaQuotaFissaAnnua: &MateriaEnergiaQuotaFissaAnnua 65.4
    TariffaF1: &tariffaf1 0.0869847
    TariffaF2: &tariffaf2 0.0869847
    TariffaF3: &tariffaf3 0.0869847
    # Trasporto costi unitari
    KwContatore: &KwContatore 6
    TrasportoQuotaFissaAnnua: &TrasportoQuotaFissaAnnua 20.4000
    TrasportoQuotaPotenzaAnnua: &TrasportoQuotaPotenzaAnnua 20.8800
    TrasportoQuotaEnergia: &TrasportoQuotaEnergia 0.00833000
    # Oneri Di Sistema costi unitari 
    OneriDiSistemaQuotaEnergia: &OneriDiSistemaQuotaEnergia 0.041817
    # Accisa costi unitari  
    Accise: &accise 0.0227 
    #IVA
    Iva: &iva 10      
  ##--------------------- IMPOSTAZIONI DEL PACKAGE ---------------------##     
    
</xmp>

-
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

