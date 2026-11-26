# EXPERIMENT NO. 4 – HALF WAVE AND FULL WAVE BRIDGE RECTIFIERS

| **Name: MOHAMED SHAJID A** | | **Reg. No.:25013425** | |
|---|---|---|---|
| **Date:26/11/2026** | | **Batch / Section:19EE305-26ODJ102** | |

---

## AIM

To study the half wave and full wave bridge rectifiers with and without filter and to observe their input and output waveforms using Proteus.

## COMPONENTS AND EQUIPMENT REQUIRED

| S. No. | Components / Equipment |
|:---:|:---|
| 1 | Diodes |
| 2 | Resistor (load) |
| 3 | Capacitors (filter) |
| 4 | Step-down transformer |
| 5 | Voltmeter |
| 6 | Ammeter |
| 7 | Breadboard |
| 8 | CRO |
| 9 | Connecting wires |
| 10 | Simulation software – Proteus Design Suite |

## THEORY

A rectifier changes AC to DC and is an essential part of a power supply. The unique property of a diode, permitting current to flow in only one direction, is utilised in rectifiers.

### Half wave rectifier

Mains supply is applied to the primary of the step-down transformer. All the positive half cycles of the stepped-down AC supply pass through the diode and all the negative half cycles are eliminated. The peak value of the output voltage is less than the peak value of the input voltage by about 0.6 V because of the voltage drop across the diode. For a half wave rectifier, **Vrms = Vm/2** and **Vdc = Vm/π**, where Vrms is the RMS value of the output, Vdc is the average value of the output and Vm is the peak value of the output.

### Full wave bridge rectifier

During the positive half cycle of the secondary voltage, diodes D1 and D3 are forward biased and D2 and D4 are reverse biased, so current flows through the secondary winding, D1, the load resistor and D3. During the negative half cycle, D2 and D4 are forward biased and D1 and D3 are reverse biased, so current flows through the secondary winding, D2, the load resistor and D4. In both half cycles the current through the load resistor is in the same direction. The peak output voltage is less than the peak input voltage by about 1.2 V due to the drop across two diodes. For a full wave bridge rectifier, **Vrms = Vm/√2** and **Vdc = 2Vm/π**.

### Filters

All rectifier outputs contain a considerable amount of ripple in addition to the DC component. To remove the AC components, a filter is connected at the output of the rectifier. Capacitor input, choke input, RC, CRC, LC and CLC filters are commonly used; the capacitor input filter is the simplest and cheapest. A high-value capacitor C is connected in shunt with the load resistor RL. The capacitor charges to the peak voltage when a half cycle appears at the output. After the peak, the capacitor discharges slowly through RL, since the diode is reverse biased by the capacitor voltage. Before the capacitor voltage drops substantially, the next output cycle arrives and the capacitor recharges to the peak.

## PROCEDURE

1. Wire up the half wave rectifier circuit without capacitor after testing all the components.
2. Switch on the mains supply. Observe the transformer secondary voltage waveform and the output voltage waveform across the load resistor simultaneously on the CRO.
3. Connect the capacitor filter across the load and observe the waveforms. Repeat for different capacitor values.
4. Repeat the above steps for the full wave bridge rectifier.
5. Simulate both rectifiers, with and without filter, in Proteus and capture the input and output waveforms on the virtual oscilloscope.

## CIRCUIT DIAGRAMS

### Half wave rectifier without filter

<img width="929" height="480" alt="Screenshot (68" src="https://github.com/user-attachments/assets/212fc11f-1756-403e-80a5-678226492016" />

**Figure 1:** Half wave rectifier without filter

### Half wave rectifier with filter

<img width="808" height="749" alt="Screenshot (72" src="https://github.com/user-attachments/assets/724eed44-622d-4ab7-8e87-7fd01be1e7ff" />

**Figure 2:** Half wave rectifier with filter

### Full wave bridge rectifier without filter

<img width="1042" height="378" alt="Screenshot (74" src="https://github.com/user-attachments/assets/ee975f4f-be85-4476-b5c9-ba33c5372905" />

**Figure 3:** Full wave bridge rectifier without filter

### Full wave bridge rectifier with filter

<img width="1092" height="752" alt="Screenshot (75" src="https://github.com/user-attachments/assets/b7179666-c6bf-4d98-8e7d-c31441e2d71a" />

**Figure 4:** Full wave bridge rectifier with filter

## SIMULATION AND WAVEFORMS USING PROTEUS

Build each rectifier in Proteus, with and without the capacitor filter. Use the virtual oscilloscope to display the input (secondary) and output waveforms together, and paste the screenshots below.

### Half wave rectifier without filter – waveform

<img width="752" height="260" alt="Screenshot (67" src="https://github.com/user-attachments/assets/2214d583-9a19-48be-8be8-ee5de27558af" />

**Figure 5:** Proteus waveform – half wave rectifier without filter

### Half wave rectifier with filter – waveform

<img width="756" height="257" alt="Screenshot (69" src="https://github.com/user-attachments/assets/05c4ac34-bcdd-417d-8b81-10b149f638ed" />

**Figure 6:** Proteus waveform – half wave rectifier with filter

### Full wave bridge rectifier without filter – waveform

<img width="752" height="449" alt="Screenshot (73" src="https://github.com/user-attachments/assets/7334e87f-bde4-4dc2-ad8d-4803fe25cc91" />

**Figure 7:** Proteus waveform – full wave bridge rectifier without filter

### Full wave bridge rectifier with filter – waveform

<img width="758" height="444" alt="Screenshot (76" src="https://github.com/user-attachments/assets/721fc0b4-8052-4b63-85fc-50e7edc8611b" />

**Figure 8:** Proteus waveform – full wave bridge rectifier with filter

## FORMULAE

### A. Half wave rectifier

- Average (DC) voltage: **Vdc = Vm / π**
- Average (DC) current: **Idc = Im / π**
- RMS voltage: **Vrms = Vm / 2**
- RMS current: **Irms = Im / 2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 1.21**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 40.6 %**
- Form factor: **FF = Vrms / Vdc = 1.57**
- Peak factor: **PF = Vm / Vrms = 2**
- Peak inverse voltage: **PIV = Vm**

### B. Full wave bridge rectifier

- Average (DC) voltage: **Vdc = 2Vm / π**
- Average (DC) current: **Idc = 2Im / π**
- RMS voltage: **Vrms = Vm / √2**
- RMS current: **Irms = Im / √2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 0.482**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 81.2 %**
- Form factor: **FF = Vrms / Vdc = 1.11**
- Peak factor: **PF = Vm / Vrms = √2 = 1.414**
- Peak inverse voltage: **PIV = Vm**

### C. With capacitor filter

- Half wave: **γ = 1 / (2√3 f C RL)**
- Full wave bridge: **γ = 1 / (4√3 f C RL)**

### D. Regulation

- **% Regulation = (VNL − VFL) / VFL × 100**

Vm – peak output voltage; Im – peak load current (Im = Vm / RL); RL – load resistance; f – supply frequency (50 Hz); C – filter capacitance; VNL – no-load voltage; VFL – full-load voltage.

## RESULT

Thus, the input and output waveforms of the half wave and full wave bridge rectifiers with and without filter were observed using Proteus.
