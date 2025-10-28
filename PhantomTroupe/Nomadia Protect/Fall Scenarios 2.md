# Sit on the Chair Test - Free Fall Related to Heights

|  Backoffice Sensitivity   | iOS (Flutter Testflight Version) | Android Java (Play Store Version) Reversed Sensibility | Comments                           |
| :-----------------------: | :------------------------------: | :----------------------------------------------------: | :--------------------------------- |
| **10** (High Sensitivity) |              **OK**              |                       **1** - OK                       | Not triggered for the applications |
|           **9**           |              **OK**              |                       **2** - OK                       |                                    |
|           **8**           |              **OK**              |                       **3** - OK                       |                                    |
|           **7**           |              **OK**              |                       **4** - OK                       |                                    |
|           **6**           |              **OK**              |                       **5** - OK                       |                                    |
|           **5**           |              **OK**              |                       **6** - OK                       |                                    |
|           **4**           |              **OK**              |                       **7** - OK                       |                                    |
|           **3**           |              **OK**              |                       **8** - OK                       |                                    |
|           **2**           |              **OK**              |                       **9** - OK                       |                                    |
|  **1** (Low Sensitivity)  |              **OK**              |                      **10** - OK                       |                                    |
# Fall Detection and Behavior Test Results

## Test Environments & Global Notes

| Platform | OS Version | NPM Version | Global Notes |
| :--- | :--- | :--- | :--- |
| **iOS** | 18.5 | 3.0.2-49 | Location permission: **No popup** separately for changing the location services to "Always Allow". |
| **Android** | 16 | 3.0.1-46 | Phone Number field automatically selects **France** (still not India as expected). |

---

## Free Fall - Jump (Keeping Mobile Opposite of Impulse Foot)

| Backoffice Sensitivity | iOS (Flutter Testflight Version) | Android Java (Play Store Version) (Reverse Sensibility) | Comments |
| :---: | :---: | :---: | :--- |
| **10** (High Sensitivity) | OK | OK | |
| **9** | OK | OK | |
| **8** | OK | OK | |
| **7** | OK | OK | |
| **6** | OK | OK | |
| **5** | OK | OK | |
| **4** | OK | OK | |
| **3** | OK | OK | |
| **2** | OK | OK | |
| **1** (Low Sensitivity) | OK | **KO** | Alarm is triggered on **Java Application consistently**. |

---

## Free Fall (Sitting on the Floor)

| Backoffice Sensitivity | iOS (Flutter Testflight Version) | Android Java (Play Store Version) | Comments |
| :---: | :---: | :---: | :--- |
| **10** (High Sensitivity) | OK | **1** - OK | |
| **9** | OK | **2** - OK | |
| **8** | OK | **3** - OK | |
| **7** | OK | **4** - OK | |
| **6** | OK | **5** - OK | |
| **5** | OK | **6** - OK | |
| **4** | OK | **7** - OK | |
| **3** | OK | **8** - OK | |
| **2** | OK | **9** - **KO** | Out of 4 times, **Prealarm triggered once on Java**. |
| **1** (Low Sensitivity) | OK | **10** - OK | Out of 10 times Prealarm **not triggered on both Devices**. |

---

## iOS Fall Detection Matrix

|  Backoffice Sensitivity   | Sitting on Chair | Sitting on Floor | Mobile Out of Pocket to Desk | Bag to Desk | Jump over Pit (70 cm) |
| :-----------------------: | :--------------: | :--------------: | :--------------------------: | :---------: | :-------------------: |
| **10** (High Sensitivity) |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **9**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **8**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **7**           |        OK        |        OK        |              OK              |     OK      |                       |
|           **6**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **5**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **4**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **3**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|           **2**           |        OK        |        OK        |              OK              |     OK      |          OK           |
|  **1** (Low Sensitivity)  |        OK        |        OK        |              OK              |     OK      |          OK           |

---

## Android Fall Detection Matrix

|  Backoffice Sensitivity   | Sitting on Chair | Sitting on Floor | Mobile Out of Pocket to Desk |     Bag to Desk      | Jump over Pit (70 cm) | Comments                                                                                                            |
| :-----------------------: | :--------------: | :--------------: | :--------------------------: | :------------------: | :-------------------: | :------------------------------------------------------------------------------------------------------------------ |
| **10** (High Sensitivity) |        OK        |      **KO**      |              OK              |          OK          |          OK           | **1 out of 5 times** the prealarm is triggered for Android while sitting on the floor                               |
|           **9**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **8**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **7**           |        OK        |        OK        |              OK              | **OK** with comments |          OK           | While placing the bag on the floor - it triggered once (maybe due to the force) but **not reproduced consistently** |
|           **6**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **5**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **4**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **3**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|           **2**           |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |
|  **1** (Low Sensitivity)  |        OK        |        OK        |              OK              |          OK          |          OK           |                                                                                                                     |