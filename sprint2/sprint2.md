Com veiem amb el ls -l apareixen correctament els cinc fitxers amb el missatge.

<img width="664" height="201" alt="Captura de pantalla de 2026-10-27 13-44-34" src="https://github.com/user-attachments/assets/f0c8b6ff-1f11-4eb4-8426-659ad69c9f53" />


Quan fem la comanda de pstree ens apareixen els sospitosos que penjen de systemd i com veiem apareixen tots.
<img width="355" height="164" alt="Captura de pantalla de 2026-10-27 13-47-13" src="https://github.com/user-attachments/assets/7b87c0a6-3cf8-4d30-acf5-c9ec158f44a2" />

<img width="344" height="132" alt="Captura de pantalla de 2026-10-27 13-48-20" src="https://github.com/user-attachments/assets/699dbcff-3146-4998-a3a0-3d17ae46bc22" />

<img width="410" height="112" alt="Captura de pantalla de 2026-10-27 13-48-28" src="https://github.com/user-attachments/assets/e7611c0f-023a-48dc-b9bb-eb8b5d47afc8" />


Quan fem un top a la terminal com podem veure el minador es troba a la part de dalt de tot ordenat per CPU.
<img width="1213" height="975" alt="Captura de pantalla de 2026-10-27 13-50-00" src="https://github.com/user-attachments/assets/f6832c69-b0cd-4dac-89c5-2cbe08236fa5" />


He buscat tots els sospitosos alhora filtrant-ho per les columnes que m'interessen i he mirat quin és el pare i he posat el numero PPID que m'ha sortit.
<img width="1080" height="497" alt="Captura de pantalla de 2026-10-27 13-54-23" src="https://github.com/user-attachments/assets/92451f96-da95-4230-b12b-070de459d995" />


Com veiem la seqüència es mostra correctament de totes les comandes amb la terminal 2 que de mentres mostra el progrès.
<img width="986" height="524" alt="Captura de pantalla de 2026-10-27 13-58-54" src="https://github.com/user-attachments/assets/32691b06-82e1-44c1-8225-39963f7343f0" />


He fet el top amb els tres processos i com veiem esta la prioritat pujada de descarrega.sh que es mostra a top correctament.
<img width="985" height="394" alt="Captura de pantalla de 2026-10-27 14-10-36" src="https://github.com/user-attachments/assets/73cf2cd1-74f4-420a-905d-c73fae42fe6f" />


Com veiem he fet les comandes següents pero com espia ignora el kill i mostra un missatge haurem de fer-ho amb un -9 per poder matar el procés.
<img width="658" height="271" alt="Captura de pantalla de 2026-10-27 14-16-21" src="https://github.com/user-attachments/assets/2fdafca6-bc58-4c0a-8d66-13589c68609f" />

I com veiem aquí també mirem el ID de nocturn i ho provem de parar amb un STOP pero si mirem el seu estat segueix estan actiu i ho farem en un -CONT per a poder parar-ho i com veiem ja es parara.
<img width="704" height="290" alt="Captura de pantalla de 2026-10-27 14-18-40" src="https://github.com/user-attachments/assets/63e250b6-6e56-4ac4-91cb-e1deb0175986" />


Executem la comanda i com veiem la terminal 2 es mostra la descarrega com a COMPLETADA.
<img width="958" height="578" alt="Captura de pantalla de 2026-11-09 10-34-39" src="https://github.com/user-attachments/assets/eea762f5-100e-4380-be6b-fd75a072ad0f" />
