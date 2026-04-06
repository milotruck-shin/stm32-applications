This application is a dummy code for testing interrupts for CAN protocol (STM32H755ZI)
- CAN RxFifo0 interrupt with LED toggling and printing to Serial terminal
- TIM16 interrupt that fires every 0.5ms

**FDCAN basic parameters

| Frame Format  | Classic Mode  |
| Mode  | Internal Loopback Mode  |
| Nominal SJW  | 40  |
| Data Prescaler  | 1  |
| Data SJW | 8  |
| Data TimeSeg1  | 15  |
| Data TimeSeg2  | 8  |
| Rx Fifo0 Elmts Nbr  | 8  |
| Rx Fifo0 Elmt Size  | 8 bytes data field  |
| Tx Events Nbr  | 16  |
| Tx Events Size  | 16  |
| Tx Elmt Elmt Size  | 8 bytes data field  |
<br>
**FDCAN bit timings parameters
| Nominal Prescaler  | 1  |
| Nominal TimeSeg1  | 79  |
| Nominal TimeSeg2  | 40  |
<br>
**USART3 Mode and Configuration
| Mode   | Asynchronous  |
| GPIO   | PD8 & PD9  |
| Baud Rate   | 115200 Bits/s  |
<br>












