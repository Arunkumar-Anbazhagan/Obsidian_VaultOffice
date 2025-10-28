# 🚀 Nomadia Field Service Mobile (NFS) v1.7.6

> **Release Type:** Patch
> **Release Date:** October 30, 2025
> **Approx. Size:** 178 MB
> **Compatibility:** Android & iOS (Recent Versions)

## ✨ Highlights: New Features and Key Improvements

Version 1.7.6 introduces two significant enhancements powered by intelligence and reliability checks to streamline fieldwork and documentation.

| Feature | Description | Impact |
| :--- | :--- | :--- |
| **AI Remark Correction** | Improves the quality of intervention reports by suggesting clear and contextual corrections to technician remarks. Includes the ability to easily undo changes. | Ensures higher quality documentation and less time spent on corrections by the back office. |
| **Image Quality Check** | Automatically verifies the sharpness and compliance of photos taken during interventions. | Reduces the number of image rejections, increasing overall report reliability and data integrity. |

---

## 🛠️ Fix Details and Minor Improvements

This patch includes several quality-of-life improvements focused on user experience and configuration flexibility.

| #     | Improvement / Fix                     | Details                                                                                                                                               |
| :---- | :------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1** | **Option to Hide WhatsApp**           | Adds an option to prevent offering users the ability to start phone calls via the WhatsApp application.                                               |
| **2** | **Documents Tab Visibility**          | The "Documents" tab is now automatically hidden if the user cannot add documents *and* the intervention currently contains none.                      |
| **3** | **Reduced Offline Bar Intrusiveness** | The orange offline status bar is now less intrusive, improving screen readability when the connection is lost.                                        |
| **4** | **Support Email Removal**             | The direct support email address has been removed from the application's settings.                                                                    |
| **5** | **Dashboard Clarity**                 | Uncompleted, canceled, and abandoned interventions are now more clearly indicated and distinguished on the technician's dashboard.                    |
| **6** | **Mission Creation UX**               | The process for creating a new mission has been simplified with better-organized fields and the removal of the step progress bar.                     |
| **7** | **Barcode-less Task Scan**            | Technicians can now scan a planned task without needing to know the barcode in advance, allowing the code to be set directly during the intervention. |

---

## 🔒 Quick Notes for Administrators

* **WhatsApp Permissions:** After deployment, remember to check and adjust the display permissions for the WhatsApp calling option if you intend to hide it for your users.
* **Support:** For help or issues, please open a ticket from the **admin portal**.

# AI Features Demo: Speech-to-Text for Survey JS Auto-Fill

## 1. Feature Overview
* [cite_start]**Core Functionality:** Converts spoken voice input into text and then uses that text to **automatically fill** fields within a Survey JS form[cite: 1].
* [cite_start]**User Interface:** A new **mic icon** is available within the Survey JS form to launch the feature[cite: 4].
* [cite_start]**Process Flow:** Speech-to-Text Recognition (App) → Send Text to AI Web Service Endpoint → Survey Auto-Fill Conversion (AI Service)[cite: 26].
* [cite_start]**Input Parameters (to AI Service):** Includes the `Client ID`, the device's set `language` (e.g., English), the `Survey JS form` data, and the `text from audio` (the recognized transcript)[cite: 28, 29, 31, 32].
* **Key Capabilities:**
    * [cite_start]Supports **continuous listening** for extended speech[cite: 23].
    * [cite_start]Works for almost every type of Survey JS form field, including **date, time, email, phone number, and matrix dynamic types**[cite: 36].
    * [cite_start]Operates in **offline mode**[cite: 38].
* [cite_start]**User Experience:** The user can **review the transcribed text** before sending it to the AI endpoint for auto-fill conversion[cite: 25]. [cite_start]A confirmation dialog appears if the user tries to exit without saving the form[cite: 37].

---

## 2. Job Report Details (Used for Demonstration)

The following details were extracted by the AI feature from the voice input describing a completed job:

* [cite_start]**Job Date & Time:** October 6, 2025, finished at 12:45 PM (started 2 hours earlier)[cite: 13].
* [cite_start]**Customer Presence:** Customer was present for a portion of the job[cite: 13].
* [cite_start]**Main Problem:** Repair of a **malfunctioning hydraulic pump**[cite: 14].
* **Other Issues Identified:**
    * [cite_start]A **meter** was displaying inconsistent readings[cite: 14].
    * [cite_start]A **control valve** was stuck[cite: 15].
    * [cite_start]The equipment was initially **partially functional** and working intermittently, causing pressure fluctuations[cite: 16, 17].
    * [cite_start]The hydraulic pump fluid was **dark brown**[cite: 14].
* **Operations Performed:**
    * [cite_start]Removal and cleaning of the pump[cite: 17].
    * [cite_start]Checking of electrical connections[cite: 17].
    * [cite_start]**Replacement of the control valve** (caused delay)[cite: 17, 18].
    * [cite_start]**Recalibration of the meter**[cite: 17].
* [cite_start]**Measurements:** Temperature at the pump outlet was **45°C** (within the normal range)[cite: 18].
* [cite_start]**Time Spent On-site:** Approximately **one hour and a half**[cite: 18].
* **Customer Feedback & Follow-up:**
    * [cite_start]**Satisfaction:** Generally satisfied but remained cautious[cite: 19].
    * [cite_start]**Technician Rating:** 4 out of 5[cite: 19].
    * [cite_start]**Requested Follow-up:** A check-up during the **second week of next month** to confirm stability[cite: 20].
    * [cite_start]**Contact Info:** E-mail: `ABC@gmail.com`, Phone: `0987654321`[cite: 21].