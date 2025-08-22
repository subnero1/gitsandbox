---
name: Support card template [Gen 4X modem]
about: Create a support card for a Gen 4X modem.
title: <Customer Name>_<Model No>_<Modem Serial No>
labels: support card
assignees: MdFaez

---

## Support card

## A. Product Record (To be updated by Production Team)

- Serial number:
- Model number:
- Link to works order (Github):
- Shipping date:
- End Customer:
- Default Static IP Address:
- Last known Software Version:
- SWIS Version (if applicable):



## B. Build List (To be updated by Production Team)

Please fill up the serial numbers for each subassembly and module in this section.

>> Note: Delete the part numbers or sections which are not applicable.

- ASDS-A-02x - Analog-Digital Electronics Stack:

  - MCM-00000001 - Matching circuit module:

  - TXM-00000001 - Transmit Module:

  - RXM-00000001 - Receiver Module:

  - PMM-0000009 - Power Management Module:
 
  - BBM-0000001_F - BBM Full (Buck/Boost):
 
  - DAQM-0000011 - GroguDAM:
 
  - GIM-0000002 - Grogu Interface Module:
    
- [ ] Is this modem a Silver edition? If yes, fill up the serial numbers for:
  - Compulab imx8 Module:
  - CBM-0000001 - Nevarro:
       
- [ ] Is this modem a Gold edition? If yes, fill up the serial numbers for:
  - Jetson Orin Nano:
  - Hadron Carrier Board:
  - NVME:

- [ ] How many channels this modem has: 1 / 2 / 4
- [ ] Frequency band: MF (T257) / HF (T582) / LF (T313)
- [ ] Which storage option: 256 GB / 1 TB

- [ ] Is this an SC and an Aluminium modem? If yes, fill up the serial numbers for:
  - XF-BEC-SCAL-01x - Bulkhead Endcap:
  - EXT-SCAL-STD-01x - External Assembly:
  - XF-TEC-SCAL-01x - Transducer Endcap:

- [ ] Is this an SC and a Stainless Steel modem? If yes, fill up the serial numbers for:
  - XF-BEC-SCST-01x - Bulkhead Endcap:
  - EXT-SCST-STD-01x - External Assembly:
  - XF-TEC-SCST-01x - Transducer Endcap:
    
     
 
### Optional Upgrades (Delete if not applicable):
- [ ] Does this have a coprocessor? If yes, Co-processor serial number:
- [ ] Does this modem have a transducer with a cable length that is not 5m? If yes, state the length:
- [ ] Does this modem have more than 4 channels? If yes, state the number of channels:



## C. Pre-production QC (To be updated by QC Manager)

[Refer to Pre-production QC Guidelines Document](https://github.com/subnero1/wnc-production/blob/17-Mar-2025-updates/Documentation/QC/Internal%20QC%20Guidelines.markdown) and fill up the checklist below.

- Internal QC conducted by (Please specify name of officer): Esther
- Overall Status (Pass/Fail):
- Inspection Date:
- [ ] Is the modem build list filled out (Section B)?
- [ ] Is the ASDS serial number label present and affixed to the device?
- [ ] Are there no signs of rust or corrosion on the electronic stack?
- [ ] Are tamper-proof markings present on all visible screws?
- [ ] Are the electrical harnesses neatly secured with cable ties?
- [ ] Does a gentle tug on all visible electrical harnesses not cause any disconnection from the PCB?
- [ ] Does a vigorous shake of the electronic stack not cause any items to fall out?
- [ ] Is the chassis connection lead present?
- [ ] Does each groove contain a greased o-ring sitting uniformly without damage, tear, or debris?

## D. Production test (To be updated by Production Team)
Please check off the tests only if they have passed. 
If any of the tests have failed, please specify the test failed and request for assistance from the relevant engineer.

### D1. Bench tests

- Overall Status (Pass/Fail):
- Remarks:
  
- [ ] A1 - Vacuum Test (SC / MC modem)
- [ ] A2 - Idle Current Draw Measurement
- [ ] A3 - DHCP IP Assignment Verification
- [ ] A4 - POST status
- [ ] A5 - Noise Level Check
- [ ] A6 - Sleep Mode Test & Current Measurement
- [ ] A7 - CoProcessor Tx/Rx Test (Only for Co-processor modems)
- [ ] A8 - RS232 Loopback Test
- [ ] A9 - Verification Script Test

### D2. Bucket test

- Overall Status (Pass/Fail):
- Remarks:
  
- [ ] B1 - Power Cycle Test (30 cycles)
- [ ] B2 - Receive Bandwidth Sweep Test (2kHz steps)
- [ ] B3.1 - Receive Signal Level Check (Gain level: 36dB)
- [ ] B3.2 - Receive Signal Level Check (Gain level: 12dB)
- [ ] B3.3 - Receive Signal Level Check (Gain level: 0dB)
- [ ] B3.4 - Receive Signal Level Check (Gain level: -120dB)
- [ ] B4 - Low Power Level Transmit Sweep Test (12dB steps)

### D3. Tank tests

- Overall Status (Pass/Fail):
- Remarks:

- [ ] C1 - High Power Level Transmit Sweep Test (6dB steps)
- [ ] C2 - Bi-directional Communication Test
- [ ] C3 - Bi-directional File Transfer Test
- [ ] C4.1 - Full Power Transmission Test [CONTROL frame]
- [ ] C4.2 - Full Power Transmission Test [DATA frame]
- [ ] C5 - Bi-directional Ranging Measurement

### D4. Calibration and Post-calibration

- [ ] D1 - Calibration Test
- [ ] D2 - Post-Calibration Clean Up

## E. Software configuration & delivery-specific tests (To be updated by Software Engineer)
To be updated for SWIS orders or project orders.

- Software version number:
- Test Outcome (Pass/Fail):
- Installation Date:
- Remarks:

## F. Pre-shipping QC Checklist (To be updated by QC Manager)

[Refer to Pre-shipping QC Guidelines](https://github.com/subnero1/wnc-production/blob/17-Mar-2025-updates/Documentation/QC/External%20QC%20Guidelines.markdown) and fill up the checklist below.

- QC conducted by (Please specify name of officer): Adi
- Overall Status (Pass/Fail):
- Final Inspection Date:

### General Checklist:
- [ ] Are all support card details from Sections A-E filled in this document?
- [ ] Does the support card folder on Google Drive contain the `modem-serial.pdf`, `modem-serial.h5`, `modem-serial_VS.rtf,` and user manual for this modem?
- [ ] Does the `modem-serial.pdf` file display the correct serial number, PSD plot, and source level plot?
- [ ] Does the user manual display the correct details? (Check Page 1, Appendix A, and Appendix B).
- [ ] Does the `modem-serial_VS.rtf` file display the correct model number and serial number, show “OK” for POST status, and have no “FAIL” in any test results?
- [ ] Is the modem physically similar to the standard modem shown in the QC guidelines?
- [ ] When the modem is shaken vigorously, does nothing come loose or make any internal noise?
- [ ] Does the modem have the correct identification label? <br />e.g. ```Model No: WNC-M25MSS4x Serial No: 20250200009 Static IP: 192.168.42.73```.
- [ ] (Customer-specific requirements or SWIS orders) Are the configuration test scripts captured in the support card?

### If the modem is an SC/MC modem (Delete section where not applicable):
- [ ] Is the Bulkhead connector fitted with a dummy plug?
- [ ] Are all external surfaces of the modem clean and free from visible damage?
- [ ] When the cage legs and eye bolts are hand-twisted, do they remain secure and not come loose?
- [ ] When the vent screw cap is hand-twisted, does it remain tight and not come loose easily?
- [ ] Are there 2 Subnero logo stickers placed at the correct locations?
- [ ] Are the 3 hydrophones are tagged with the right labels i.e. `CH2`, `CH3`, `CH4`?

### If the modem is an OC modem (Delete section where not applicable):
- [ ] Are the interfacing power and Ethernet harnesses `W-0000213` and `W-0000211` connected to the modem?
- [ ] Is the transducer soldered to the modem, and the transducer label covered with heat shrink?
- [ ] Is there an o-ring present on the transducer?
- [ ] Is an interface plate securely fixed to the bottom of the modem?
- [ ] Is the chassis connection lead present?


## G. Support (To be updated by Support Engineer)

- Link to Return-to-repair or Return-to-upgrade order (Github):
- Link to Inspection Report (Github):

#### G1. Additional information not present in the report:

- 
-
