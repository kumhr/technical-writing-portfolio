# Technical Data Sheet: 36V Li-ion Battery Pack

## 1. Electrical Specifications

| Parameter | Value | Notes |
| :--- | :--- | :--- |
| **Nominal Voltage** | 36.0 V | |
| **Capacity** | 14.0 Ah (504 Wh) | |
| **Charge Cut-off Voltage** | 42.0 V | ±0.5V |
| **Discharge Cut-off Voltage** | 30.0 V | BMS Protection |
| **Max Charge Current** | 4.0 A | Using OEM Charger |

## 2. Pinout Configuration

| Pin | Function | Description |
| :---: | :--- | :--- |
| 1 | **BAT+** | Positive Power Terminal |
| 2 | **BAT-** | Negative Power Terminal |
| 3 | **CAN High** | Communication Bus |
| 4 | **CAN Low** | Communication Bus |

> [!CAUTION]
> **ELECTRICAL HAZARD:** Do not bridge Pin 1 and Pin 2 with metallic objects. Short-circuiting may cause battery fire or permanent BMS damage.