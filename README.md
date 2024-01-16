Fork di https://github.com/ibielopolskyi/smartthings_fridge_camera
Integrazione per aggiungere entità Camera del Frigorifero Samsung Side by Side Family Hub ad Home Assistant
Verranno aggiunte tre entità:
camera.top
camera.middle
camera.bottom

Se avete il frigorifero con una sola telecamera centrale aprire il file
/custom_components/samsung_frigorifero_familyhub/camera.py
e commentare le righe 53 e 54

**INSTALLAZIONE CON HACS**:

1) Andare su HACS e cliccare sui tre puntini (hamburger menu) in alto a destra e poi su Archivi digitali personalizzati
<img width="202" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/a47e3294-6c7f-4376-b5ca-010d09043d37">

2) Inserire la url https://github.com/antoweb/smartthings_camera_frigorifero in Archivio digitale

4) Selezionare categoria Integrazione
<img width="269" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/2e342683-bed7-4c66-a744-b9eefe7440a3">

5) Cliccare su aggiungi
6) Chiudere con la x se è comparso l'archivio nell'elenco
<img width="317" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/717454a9-016c-4186-ab3e-8ac650dfda58">

7) Su Hacs digitare family hub nella casella di ricerca
<img width="286" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/b8840c79-75c7-4e10-adce-450278680030">

8) Cliccare sopra e si aprirà pagina seguente
<img width="362" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/f7ba4ff1-7ed3-40b6-ba94-71da1f5d8f81">

9) Cliccare su scarica in basso a dx
<img width="115" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/22b1517c-328e-450b-906a-52c2085da09a">

10) Di nuovo su scarica
   <img width="263" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/7af7882e-2306-4a7d-bd3e-8f76581beda9">
   
11) DOvreste avere la cartella samsung_frigorifero_familyhub in /config/custom_components
<img width="218" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/9a272b62-ff19-4750-a482-77da827ea382">

12) Andare su Menu/Integrazioni
<img width="301" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/ef2e55d7-f2c2-4d9a-b29f-620cccf50ea5">

13) Cliccare su aggiungi integrazione in basso a dx
<img width="125" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/29e4c84d-2b46-4677-8bb2-e59f2ddea4ce">

14) Digitare Frigorifero o FamilyHub nella casella di ricerca
<img width="232" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/dc7798bf-6102-4dd4-a673-7840c8f49909">

15) Cliccare sull'integrazione per aggiungerla ad Home Assistant

16) Riavviare Home Assistant
17) Procedere alla configurazione come descritto sotto dal punto 7)


**INSTALLAZIONE SENZA HACS**:
1) Scaricare il codice master
2) Scompatare il contenuto e salvare la cartella samsung_frigorifero_familyhub in /config/custom_components di HA
3) Riavviare HA
4) Dopo il riavvio andare su Integrazioni e cliccare su aggiungi integrazione
<img width="125" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/29e4c84d-2b46-4677-8bb2-e59f2ddea4ce">

5) Digitare Frigorifero o FamilyHub nella casella di ricerca
<img width="232" alt="image" src="https://github.com/antoweb/smartthings_camera_frigorifero/assets/32364871/dc7798bf-6102-4dd4-a673-7840c8f49909">

6) Cliccare sull'integrazione per aggiungerla ad Home Assistant

7) Verrò chiesto token e device id
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/7def7960-2a0e-4127-a599-64018482d2ca)

8) Per recuperare il token andare su: https://account.smartthings.com/tokens col proprio account smartthings e abilitare tutti i dispositivi poi generare token
Generare un token (è possibile salvarselo per usi futuri perchè una vokta generato non sarà più visibile)

Per recuperare il device id andare su: https://my.smartthings.com/advanced

9) Autenticarsi con account smarthings
10) Cliccare su devices
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/703731dd-d2d4-41c6-a424-b321a4d03cd8)

11) Copiare il device id
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/325fb9f8-8460-48a0-9cb5-1db6574a962e)

Inserire i due valori richiesti nella finestra dell'integrazione
Riavviare Home Assistant
Al riavvio verranno create le entità camera visibili in Dashboard





