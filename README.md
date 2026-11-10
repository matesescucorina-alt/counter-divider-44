# Counter / Divider by 44 (0 to 43 counting sequence)

Proiect hardware realizat în cadrul facultății (ETcTI), constând într-un numărător sincron cu ciclu de 44 stări, alimentat la 5V și echipat cu bloc de oscilator selectabil și afișaj LED pe 6 biți.

## Specificații Tehnice
* **Secvență de numărare:** 0, 1, 2, ..., 42, 43, 0
* **Intrare ceas (Oscilator):** Frecvențe comutabile de 5 Hz, 220 kHz și buton de impuls manual (Tick).
* **Circuite Integrate utilizate:** 
  * 2x `SN74HC163N` (Numărătoare sincrone)
  * 1x `74HCT132` (Porți NAND Schmitt-Trigger pentru oscilator)
  * 1x `4012` (Detector de reset pentru starea 44)
  * 1x `L7805` (Regulator de tensiune)
* **Consum total estimat:** ~1.24 W

## Conținutul Proiectului
- **Scheme Electronice:** Schema bloc, oscilatorul cu celulă RC, sursa de alimentare și detectorul de reset.
- **PCB:** Layout pentru straturile Top/Bottom Copper și Silkscreen.
- **BOM (Lista de componente):** Condensatoare, rezistoare (470Ω, 10kΩ, 100kΩ), diode (1N4001) și LED-uri de 3mm.
