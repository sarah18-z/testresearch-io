### Radiation Testing: TID and SEE for DDR, NAND, eMMC, and SPI Memories

Radiation testing is crucial for evaluating the resilience of electronic components used in high-radiation environments, such as space or nuclear facilities. Two common types of tests are Total Ionizing Dose (TID) and Single Event Effect (SEE). Here’s an in-depth explanation of these tests as applied to DDR, NAND, eMMC, and SPI memories.

### Total Ionizing Dose (TID) Test

#### Objective
The TID test measures a component's resistance to cumulative ionizing radiation exposure, which can cause permanent degradation in electronic devices.

#### Procedure
1. **Exposure**: The component is exposed to a radiation source, often gamma rays from cobalt-60.
2. **Dosage**: Radiation dose is measured in rads (radiation absorbed dose), with typical test levels ranging from a few krad(Si) to several Mrad(Si).
3. **Electrical Parameter Measurement**: Electrical parameters (leakage current, threshold voltage, switching speed, etc.) are measured during and after exposure to detect degradation.
4. **Result Analysis**: The results help evaluate the component's tolerance to cumulative radiation dose and identify failure thresholds.

#### Effects on Memories
- **DDR**: Memory cells and support circuits can experience changes in leakage currents and threshold voltages, affecting data reliability.
- **NAND**: Data retention and read/write cycles may be compromised.
- **eMMC**: Degradation may manifest as read/write errors and decreased performance.
- **SPI**: Serial communication can be disrupted by changes in the electrical characteristics of the components.

### Single Event Effect (SEE) Test

#### Objective
The SEE test assesses a component's susceptibility to events caused by individual energetic particles (protons, neutrons, heavy ions) that can induce transient or permanent disruptions.

#### Types of SEE
- **Single Event Upset (SEU)**: Temporary bit flip.
- **Single Event Latch-up (SEL)**: Persistent unwanted conduction leading to overcurrent.
- **Single Event Burnout (SEB)**: Permanent damage caused by catastrophic failure.
- **Single Event Transient (SET)**: Unwanted transient pulse in a signal.

#### Procedure
1. **Exposure**: The component is exposed to a beam of energetic particles in a particle accelerator.
2. **Real-Time Monitoring**: During exposure, transient behaviors (bit flips, abnormal currents) are monitored.
3. **Post-Exposure Analysis**: Effects are analyzed to determine the nature and frequency of disruptions.

#### Effects on Memories
- **DDR**: SEUs can cause bit flips, while SELs can lead to excessive currents, potentially causing destruction.
- **NAND**: SEUs can cause read/write errors, and SELs can affect control circuits.
- **eMMC**: Susceptible to SEUs that can corrupt data and SELs that can damage memory management circuits.
- **SPI**: SETs can induce communication errors, and SEUs can corrupt configuration registers.


### Algorithms

1. **March Algorithms:**
   - **March C-:** A comprehensive algorithm for detecting various faults. Consists of sequences of write and read operations. [1]
   - **March B:** Focuses on detecting specific types of faults like stuck-at and transition faults.
   
2. **BIST (Built-In Self-Test):**
   - Embedded testing routines that run autonomously within the memory device.
   - Includes algorithms for detecting and correcting errors.

3. **ECC (Error Correction Code):**
   - Algorithms to detect and correct single-bit errors and detect double-bit errors.
   - Common ECC algorithms include Hamming Code and Reed-Solomon Code.

4. **Pattern Testing:**
   - **Checkerboard and Inverse Checkerboard:** Patterns to detect faults related to adjacent cells.
   - **Walking 1s and 0s:** Writing a single 1 or 0 in different positions to detect addressing and stuck-at faults.

5. **Data Scrambling:**
   - Algorithms that scramble data before writing it to memory to reduce the chances of pattern-sensitive faults.

#### resources : 
https://www.ijvdcs.org/uploads/524361IJVDCS2672-94.pdf
** pseudo code : **
file:///C:/Users/sarah/Downloads/5314-5328-1-PB%20(1).pdf


#### Radiation tests : 
https://www.sciencedirect.com/science/article/pii/S0273117724004769
https://theses.hal.science/tel-01954572/file/Viyas_Gupta_2017.pdf
https://nepp.nasa.gov/docuploads/4f678de9-9f55-4e2e-863df9c9f35db603/w-4_nguyen-flash%20memory.pdf

#### Nand flash memory :
https://www.ijeat.org/wp-content/uploads/papers/v2i4/D1396042413.pdf
https://patents.google.com/patent/CN111653305A/en
https://www.researchgate.net/publication/3943092_Flash_memory_built-in_self-test_using_March-like_algorithms
https://www.mdpi.com/2076-3417/12/21/10697
https://www.goodram.com/fr/blog-fr/methodes-de-detection-et-de-correction-derreurs-dans-les-memoires-de-masse/
