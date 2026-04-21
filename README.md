🤖 ROBOTTINO RILEVATORE DI GAS CON ARDUINO                                                                                                                                                                                      
📌 Descrizione                                                                                                                                                                                                                  
Questo progetto prevede la realizzazione di un piccolo sistema intelligente basato su Arduino, progettato per il monitoraggio della qualità dell’aria e la rilevazione di gas potenzialmente pericolosi. Il sistema è in grado di:
Monitorare costantemente l’ambiente circostante
Rilevare la presenza di gas come GPL, metano e fumo
Segnalare visivamente il livello di rischio tramite LED
Attivare un allarme sonoro in situazioni di pericolo
Il cuore del progetto è il sensore MQ-2, che misura la concentrazione di gas nell’aria e invia i dati ad Arduino, il quale elabora le informazioni e reagisce di conseguenza.
Funzionamento
Il sistema opera in modo continuo, leggendo i valori forniti dal sensore e classificando il livello di rischio in tre fasce:
🟢 Valore basso → LED verde acceso
L’aria è pulita, nessun pericolo rilevato
🟠 Valore medio → LED arancione acceso
Presenza moderata di gas, situazione da monitorare
🔴 Valore alto → LED rosso acceso + buzzer attivo
Livello pericoloso di gas, viene attivato l’allarme sonoro
Questo comportamento permette una lettura immediata e intuitiva dello stato dell’ambiente anche senza strumenti complessi.
Logica del sistema
Il microcontrollore:
legge i dati analogici dal sensore MQ-2
confronta i valori con soglie preimpostate
attiva i LED e il buzzer in base al livello rilevato
Schema a blocchi
[Sensore MQ-2] → [Arduino UNO] → [LED verde / arancione / rosso]
↓
[Buzzer]
👥 Distribuzione dei ruoli
Luca → programmazione codice e ricerca componenti
Niccolò →
