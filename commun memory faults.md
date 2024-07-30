| **Fault**             | **Description**                                                                                            | **DDR** | **eMMC** | **SPI** | **NAND** |
|-----------------------|------------------------------------------------------------------------------------------------------------|--------|---------|--------|--------|
| **Bit Flips/Errors**  | Single Event Upsets (SEUs) due to radiation, random bit errors from manufacturing defects or aging.        | X      | X       | X      | X      |
| **Data Retention**    | Inability to retain data due to charge leakage.                                                            | X      |         |        | X      |
| **Read/Write Errors** | Failures in reading or writing data accurately.                                                           | X      |         | X      | X      |
| **Timing Errors**     | Violations of setup and hold times, leading to metastability.                                             | X      |         | X      |        |
| **Electrical Faults** | Issues such as shorts or opens in the circuit.                                                            | X      |         |        |        |
| **Wear and Tear**     | Degradation of NAND flash memory cells due to limited write/erase cycles.                                 |        | X       |        | X      |
| **Data Corruption**   | Occurs due to sudden power loss, incomplete write operations, or firmware bugs.                           |        | X       | X      |        |
| **Controller Failure**| Failure of the integrated controller due to electrical overstress, manufacturing defects, or aging.       |        | X       |        |        |
| **Power Issues**      | Malfunctions caused by power supply fluctuations or interruptions.                                        |        | X       | X      |        |
| **Firmware Bugs**     | Improper data handling due to bugs in the eMMC controller firmware.                                       |        | X       |        |        |
| **Heat-Related Failures**| Failures due to excessive heat degrading memory cells and controller.                                   |        | X       |        |        |
| **Radiation Effects** | SEUs or TID effects causing bit flips and permanent damage.                                               | X      | X       | X      | X      |
| **Block Erase Failures** | Occurs when an entire block of memory fails to erase correctly.                                          |        |         |        | X      |
| **Retention Loss**    | Data loss over time due to charge leakage from the floating gate.                                         |        |         |        | X      |
| **Endurance Degradation** | Wear-out due to limited number of program/erase cycles.                                                |        |         |        | X      |
| **Connection Faults** | Intermittent operation or complete failure due to poor solder joints or loose connections.               |        |         | X      |        |
| **Voltage Supply Issues** | Improper read/write operations due to power supply fluctuations.                                        |        |         | X      |        |
