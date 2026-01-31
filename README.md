# Cycling Performance & Air Density Calculator

Un tool web interattivo per analizzare la velocità, la potenza e la densità dell’aria nel ciclismo, con calcolo automatico delle perdite e grafici dinamici.

## Funzionalità principali
- **Calcolo automatico della velocità a partire dalla potenza** (e viceversa)
- **Grafici dinamici**: Potenza vs Velocità e perdite per componente (Drag, Rolling, Gravity, Drivetrain)
- **Calcolo e visualizzazione VAM** (Velocità Ascensionale Media, m/h)
- **Densità dell’aria**: calcolo da temperatura, pressione, umidità/dew point
- **Calcolo della pressione atmosferica per altitudine**
- **Input compatti e moderni**
- **Link utili per Crr e Drivetrain Loss**
- **Licenza MIT**

## Parametri principali
- **Potenza (W)**: la potenza erogata dal ciclista ai pedali
- **Peso ciclista/bici (kg)**: massa totale
- **Pendenza (%)**: inclinazione della strada
- **CdA (m²)**: prodotto tra Cd (coefficiente di resistenza aerodinamica, adimensionale) e A (area frontale in m²). Es: Cd ≈ 0.88, A ≈ 0.36 m² → CdA ≈ 0.32
	- **Cd**: coefficiente di drag, misura quanto "opponi resistenza" all’aria
	- **A**: area frontale, superficie proiettata frontalmente
- **Crr**: coefficiente di rotolamento (adimensionale, tipico 0.003–0.006). [Confronta qui](https://www.bicyclerollingresistance.com/road-bike-reviews/compare)
- **Drivetrain Loss (%)**: perdita di potenza nella trasmissione ([info](https://powermetercity.com/2016/11/21/power-meter-drivetrain-power-loss/))
- **Densità aria (kg/m³)**: calcolata automaticamente o inseribile
- **Vento (km/h)**: positivo = vento contrario

## Come si usa
1. Inserisci i parametri desiderati nei campi
2. I risultati e i grafici si aggiornano in tempo reale
3. Passa tra le tab "Power vs Speed" e "Air Density" per analisi diverse

## Grafici
- **Potenza vs Velocità**: mostra la potenza necessaria per ogni velocità
- **Perdite per componente**: visualizza Drag, Rolling, Gravity, Drivetrain come curve negative

## Note tecniche
- Tutte le unità sono nel SI (kg, m, s, W, m²)
- Il campo CdA richiede il prodotto Cd × A
- I calcoli della densità aria usano la formula con pressione, temperatura e umidità (o dew point)
- Il tool è completamente client-side, non richiede installazione

## Credits
- Autore: Andrea Bonvicin
- Chart.js per i grafici
- MathJax per le formule

## Licenza

MIT License

Copyright (c) 2026 Andrea Bonvicin

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

