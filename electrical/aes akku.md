<!-- omit in toc -->
# Troubleshooting Intermittent Power Loss
<!-- omit in toc -->
## Table of content:

- [Disclaimer:](#disclaimer)
- [Document overview:](#document-overview)
- [Parameters:](#parameters)
- [Safety:](#safety)
- [Required Tools:](#required-tools)
- [Step-by-Step Instructions](#step-by-step-instructions)
- [Troubleshooting diagram:](#troubleshooting-diagram)
- [Disposal of replaced parts and batteries:](#disposal-of-replaced-parts-and-batteries)

<div style="page-break-after: always;"></div>


| Document ID | Product Model | Version | Date |  
| :--- | :--- | :--- | :--- |
| SB-AES-001 | AES Akku 35.2V | v1.1 | 2026-03-21 |

---

### Disclaimer:
> [!IMPORTANT]
>- This guide is intended for qualified technicians. The manufacturer is not responsible for injury, property damage, or product damage resulting from misuse or deviation from this procedure  

### Document overview:
> [!NOTE]
>- The purpose of this document is to serve as a troubleshooting guide for intermittent power loss in AES Akku battery systems.
>
>- The table below lists important cautions:


| Caution Symbol | Description |
| :---: | :--- |
| <img src="../images/manual.png" width="50"> | Read this manual to avoid **serious injuries** or **property damage** |
| <img src="../images/gloves.png" width="50"> | Sharp edges on chassis plugs or pinch points while using pliers. Wear protective gloves during internal wiring access. |
| <img src="../images/eyes.png" width="50"> | Danger of sparks or flying debris could lead to eye injury or blindness. |

<div style="page-break-after: always;"></div>

### Parameters:

| Parameter | Specification | Value/Limit |
| :--- | :--- | :--- |
| Nominal Voltage | Operating Voltage | 35.2V |
| Max. Charge Voltage | Cut-off Limit | 42.0V |
| Discharging Current | Max. Current | 16.5A |
| Terminal Torque | M4 Screw Torque | 1.2 Nm |
| Operating Temp. | Thermal Range | -20°C to +60°C |

---   

### Safety: 

**System:** AES Swappable Battery Interface  

 **⚠️ SAFETY CRITICAL: READ BEFORE PROCEEDING**  
 **⚠️ Omitting steps or procedures from this manual could lead to death, serious bodily injuries, or property damage.**

| Hazard Symbol | Type of Danger | Description |
| :---: | :--- | :--- |
| <img src="../images/fire.png" width="50"> | **FIRE HAZARD** | Li-ion batteries are highly flammable. Thermal runaway can release toxic gases. |
| <img src="../images/electric.png" width="50"> | **ELECTRICAL** | High Current (35.2V / 16.5A). Risk of severe arcing if shorted. **Repair only by a certified technician.** |



 * **Handling:** If the battery case is swollen, hot to the touch, or emitting a "sweet" smell, **do not proceed**. 
 * **Move the battery to a fire-safe outdoor area immediately.**  

<div style="page-break-after: always;"></div>


### Required Tools:
* Phillips Screwdriver (PH2)
* Digital Multimeter
* Needle-Nose Pliers

---

### Step-by-Step Instructions

1. **Power Isolation:** 
   Remove the battery from the vehicle to ensure the circuit is broken before inspection.

2. **Battery Visual Inspection:** 
   Visually inspect the battery for swelling, abnormally hot to the touch, or a "sweet" smell; check male contacts on the battery for carbonization (burn marks) or bent contact pins. 
   - **Action:** If any of these signs occur, **safely** dispose of the battery. 

3. **Battery Voltage Verification**
   Check the battery's State of Charge (SoC). If the indicator shows "Full," measure the voltage across the primary contacts using a Digital Multimeter.
   - **Action:** 
     - If SoC is "Full" but voltage is < 35V, the battery is defective; **replace the unit.** 
     - If voltage is > 42V, the battery is defective; **replace the unit.** 
     - If SoC is not full, charge to 100% before re-testing.

4. **Chassis Plug Inspection:**
   Examine the battery interface plug inside the bike's battery holder. Look for melting plastic or widened pin-slots.

5. **Internal Wiring Access:**
   Remove the protective cover of the battery plug using a Phillips screwdriver. Inspect the primary power leads for heat damage or brittle insulation.

6. **Mechanical Tension Test (Tug Test):**
   Using Needle-Nose Pliers, gently pull the wires at the terminal block. 
   - **Action:** If wires move, tighten the terminal block screws. Replace the cable assembly if the plug housing is scorched.

7. **Validation:**
   Reinstall the battery and perform a test drive on uneven terrain to confirm power stability.

<div style="page-break-after: always;"></div>


### Troubleshooting diagram:  

```mermaid
flowchart TD
    A[1. Isolation] --> B[2. Visual check]
    
    B -- "Bad" --> Dispose[Dispose Battery]
    B -- "OK" --> C[3. Voltage check]

    C -- "Not full" --> E[3.1 Charge]
    C -- "Faulty SoC" --> Dispose[Dispose Battery]
    C -- "In range" --> F[4. Plug Check]

    E --> E_Check[Recovers?]
    E_Check -- "No" --> Dispose
    E_Check -- "Yes" --> C

    F -- "Faulty" --> G[6.2 Replace Plug]
    F -- "Good" --> H[5. Internal Check]

    H --> I[6. Tug Test]
    I -- "Loose" --> J[6.1 Tighten Screws]
    I -- "Scorched" --> G
    
    J --> K[7. Validation Drive]
    G --> K

    style Dispose fill:#ffebee,stroke:#c62828
    style K fill:#e8f5e9,stroke:#2e7d32
```
<div style="page-break-after: always;"></div>

### Disposal of replaced parts and batteries:

> <img src="../images/WEEE.png" width="50">  E-bike batteries and electronic parts are **ELECTRICAL WASTE**. Do not throw **faulty battery** or replaced **electronic** parts in the black bin. Bring electronic waste to a specialized recycling center or contact the distributor for WEEE take-back. 