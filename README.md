Fork di https://github.com/ibielopolskyi/smartthings_fridge_camera
Integrazione per aggiungere entità Camera del Frigorifero Samsung Side by Side Family Hub ad Home Assistant
Verranno aggiunte tre entità:
camera.top
camera.middle
camera.bottom

Se avete il frigorifero con una sola telecamera centrale aprire il file
https://github.com/antoweb/smartthings_camera_frigorifero/blob/main/custom_components/samsung_frigorifero_familyhub/camera.py
e commentare le righe 53 e 54

**INSTALLAZIONE**:
1) Scaricare il codice master
2) Scompatare il contenuto e salvare la cartella samsung_frigorifero_familyhub in /config/custom_components di HA
3) Riavviare HA
4) Dopo il riavvio andare su Integrazioni e cliccare su aggiungi integrazione
5) Poi scegliere Samsung Family Hib Fridge
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/3fa10943-64c2-47a4-b25d-b58c81ca5de9)

Verrò chiesto token e device id
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/7def7960-2a0e-4127-a599-64018482d2ca)

Per recuperare il token andare su: https://account.smartthings.com/tokens col proprio account smartthings e abilitare tutti i dispositivi poi generare token
Generare un token (è possibile salvarselo per usi futuri perchè una vokta generato non sarà più visibile)

Per recuperare il device id andare su: https://my.smartthings.com/advanced
1) Autenticarsi con account smarthings
2) Cliccare su devices
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/703731dd-d2d4-41c6-a424-b321a4d03cd8)

3) Copiare il device id
![image](https://github.com/antoweb/smartthings_fridge_camera/assets/32364871/325fb9f8-8460-48a0-9cb5-1db6574a962e)

Inserire i due valori richiesti nella finestra dell'integrazione
Riavviare Home Assistant
Al riavvio verranno create le entità camera visibili in Dashboard





