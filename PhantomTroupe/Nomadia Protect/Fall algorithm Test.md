[[Fall Scenarios 2]]Fall from Ladder
# Fall Detection by Accelerometer Test Results

## Test Environments
| Platform | OS Version | NPM Version |
| :--- | :--- | :--- |
| **Android** | 15 | Java (2.3.7) |
| **iOS** | 18.5 | Testflight (3.0.2-48) |

## Prerequisite
Activate the function **Free fall** from the administration interface.

---

## Test Cases

| Ref. | Spec. | Action | Expected Result | Java (Store) Result | Java Comments | Flutter iOS Result | iOS Comments | Flutter Android Result |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **FALL.1** | S10-24,8cm | Set the sensitivity to **10** | / | / |   |   |   | / |
| | | Hold the device **30cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | Fall Triggered | **KO** | Checked different scenarios like: 1. Dropped vertically, 2. Horizontally, 3. on 90 degree, 4. Thrown from the Mentioned height. The prealarm is **not** triggered. Sometimes the prealarm is triggered when the mobile is taken from the desk and placed in the hand. | **OK** |
| | | Hold the device **20cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.2** | S9-39cm | Set the sensitivity to **9** | / | / | Java: The application triggers prealarm when the mobile is dropped from **40 cm** (approximately) | **KO** |   | / |
| | | Hold the device **45cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** |   |   |   | **OK** |
| | | Hold the device **30cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.3** | S8-53,1cm | Set the sensitivity to **8** | / | / |   |   |   | / |
| | | Hold the device **60cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | Above **50 cm**, the prealarm is triggered | **KO** |   | **OK** |
| | | Hold the device **45cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** | Not triggered | **OK** |   | **OK** |
| **FALL.4** | S7-67,1cm | Set the sensitivity to **7** | / | / |   |   |   | / |
| | | Hold the device **75cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | Triggered at **70 cm** but not above **60 cm** (like 65cm) | **KO** |   | **OK** |
| | | Hold the device **60cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.5** | S6-80,9cm | Set the sensitivity to **6** | / | / |   |   |   | / |
| | | Hold the device **85cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** |   | **KO** |   | **OK** |
| | | Hold the device **65cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.6** | S5-94,1cm | Set the sensitivity to **5** | / | / |   |   |   | / |
| | | Hold the device **100cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | When the mobile is thrown from the same height the prealarm is **not** triggered | **KO** |   | **OK** |
| | | Hold the device **85cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.7** | S4-107,9cm | Set the sensitivity to **4** | / | / |   |   |   | / |
| | | Hold the device **115cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | Triggers on Free fall   | **KO** |   | **OK** |
| | | Hold the device **100cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered |   |   | **OK** |   |   |
| **FALL.8** | S3-122,1cm | Set the sensitivity to **3** | / | / |   |   |   | / |
| | | Hold the device **130cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** |   | **KO** |   | **OK** |
| | | Hold the device **115cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **OK** |   | **OK** |
| **FALL.9** | S2-136,2cm | Set the sensitivity to **2** | / | / |   |   |   | / |
| | | Hold the device **145cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** | In free fall, if the mobile is thrown with the same height, the prealarm is **not** triggered (vertically thrown) | **KO** |   | **OK** |
| | | Hold the device **125cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** | Not triggered |   |   | **OK** |
| **FALL.10** | S1-150cm | Set the sensitivity to **1** | / | / |   |   |   | / |
| | | Hold the device **155cm** above a mattress or a soft bag. Drop it. | Pre-alarm triggered | **OK** |   | **KO** |   | **OK** |
| | | Hold the device **140cm** above a mattress or a soft bag. Drop it. | No pre-alarm triggered | **OK** |   | **KO** |   | **OK** |
| **FALL.11** | | Flip the device upside down **3 times** by rotating your wrist | No pre-alarm triggering | **OK** |   | **OK** |   | **OK** |
| **FALL.12** | | Change free fall sensitivity to **5** from the administration interface | / | / |   |   |   | / |
| | | Throw the smartphone up in the air by **50cm** catch it back | No pre-alarm triggering | **KO** | Triggers the prealarm | **OK** |   | **KO** |
| | | Throw the smartphone up in the air by **10cm** catch it back | No pre-alarm triggering | **KO** | Triggers the prealarm | **OK** |   | **KO** |
| | | Put the smartphone in a bag, throw the bag onto chair, **1m** away form the chair | No pre-alarm triggering |   | Check on the below table |   |   |   |
| | | Change fall detection sensitivity to **10** from the administration interface | / | / |   |   |   | / |
| | | Throw the smartphone up in the air to the ceiling and catch it back at the level of a chair | Triggering the Fall pre-alarm on the smartphone | **OK** |   | **OK** |   | **OK** |
| | | Throw the smartphone up in the air by **50cm** catch it back | No pre-alarm triggering | **KO** | Check on the below table |   |   | **KO** |
| | | Put the smartphone wrapped bubble paper in a bag, throw the bag **3m** (4 steps) away onto the floor | Triggering the Fall pre-alarm on the smartphone |   | Need to test with Bubble paper bag |   |   |   |