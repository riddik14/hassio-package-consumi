# hassio-package-consumi
package consumi
il progetto si basa sul lavoro di Mauro Cimino che approfitto per ringraziarlo

- https://hassiohelp.eu/2019/03/02/controllo-consumi-costi/

- https://hassiohelp.eu/author/legolas08/


- Implementazione della fascia F3 e calcolo bolletta su giorno mensile e annuale, hai bisogno di un sensore che indichi il consumo in kWh da inserire nella prima parte del package - esempio di sensori comaptibili - pzem - shellyPm -
-
-
- INSTALLAZIONE

- copiare il file pkg_tariffe_luce_consumi.yaml nella cartella "/config/packages", 
- aprire il file  lovelace-dash.txt e copiare il contenuto in una card manuale dalla dashbord del tuo assistente

- alla riga 8 cambiare il sensore sensor.volt_in con il tuo volt ingresso
- alla riga 31 cambiare il sensor sensor.watt con il tuo che misura i watt istanatanei

- installare dal menu frontend di hacs:

- vertical-stack-in-card
- mini-graph-card
- banner-card
- paper-buttons-row
- state-switch




<a href="https://www.buymeacoffee.com/T1Pqksy" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/arial-black.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>
_____________________________________________________________



<img src="https://github.com/riddik14/hassio-package-consumi/blob/main/image_.png">
-
-
-
- Se il progetto ti è piaciuto clicca <a href="https://www.paypal.me/DomenicoCeccarelli">qui</a> per offrirmi un caffè

