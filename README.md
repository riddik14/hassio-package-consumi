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
- se usi shelly ti consiglio di far passare il sensore che ti indica i watt attraverso il convertitore kwh
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




<a href="https://www.buymeacoffee.com/T1Pqksy" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/arial-black.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>


- Se il progetto ti è piaciuto clicca <a href="https://www.paypal.me/DomenicoCeccarelli">qui</a> per offrirmi un caffè

