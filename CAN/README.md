# STM32H755ZI Interrupt Testing (CAN & TIM)

This application is a dummy code for testing interrupts for CAN protocol (STM32H755ZI)

## Features
* **FDCAN RxFifo0 Interrupt**: Triggers upon receiving a CAN message. The handler toggles an onboard LED and outputs the status to the Serial terminal.
* **TIM16 Interrupt**: A periodic timer interrupt configured to fire every **0.5ms** for time-critical task execution.

---

## CubeMX Configuration

### FDCAN Basic Parameters
| Parameter | Value |
| :--- | :--- |
| **Frame Format** | Classic Mode |
| **Mode** | Internal Loopback Mode |
| **Nominal SJW** | 40 |
| **Data Prescaler** | 1 |
| **Data SJW** | 8 |
| **Data TimeSeg1** | 15 |
| **Data TimeSeg2** | 8 |
| **Rx Fifo0 Elements** | 8 |
| **Rx Fifo0 Element Size** | 8 Bytes (Data Field) |
| **Tx Events Number** | 16 |
| **Tx Events Size** | 16 |
| **Tx Element Size** | 8 Bytes (Data Field) |

### FDCAN Bit Timings
| Parameter | Value |
| :--- | :--- |
| **Nominal Prescaler** | 1 |
| **Nominal TimeSeg1** | 79 |
| **Nominal TimeSeg2** | 40 |

### USART3 Mode & Configuration
Used for serial debugging and terminal output.

| Parameter | Configuration |
| :--- | :--- |
| **Mode** | Asynchronous |
| **GPIO Pins** | PD8 (TX), PD9 (RX) |
| **Baud Rate** | 115200 Bits/s |

---

## Implementation Notes
> **Note:** Since the FDCAN is set to **Internal Loopback Mode**, the controller will receive its own transmitted messages. This is ideal for testing interrupt service routines (ISRs) without needing an external CAN transceiver or bus.










