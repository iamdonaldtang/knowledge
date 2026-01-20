# TaskOn Performance-Based API Verification Guide

## **Overview** <a href="#overview" id="overview"></a>

This task template is ideal for trading competitions, allowing you to **sync points** to TaskOn. For example, users with higher trading volume can earn more points, motivating them to strive for greater achievements.The system supports two types of user identifiers:

### **Supported ID Types**

1. **Social Media Account ID**
   1. Twitter handle (e.g., taskonxyz)
   2. Discord ID (e.g., 1084460817220641111)
   3. Telegram ID (e.g., 6881505111)
   4. Email Address (e.g., [abc@gmail.com](mailto:abc@gmail.com)
2. **Blockchain Wallet Address**
   1. Supported chains: EVM, Solana, Starknet, Sui, Tron, BTC, Aptos, Nibiru

### **Integration Guide** <a href="#integration-guide" id="integration-guide"></a>

**2.1 Quick Start**

* **Demo project**: [https://github.com/Taskon-xyz/taskon-verification-demo](https://github.com/Taskon-xyz/taskon-verification-demo)
* Features:
  * **One-click** Vercel deployment
  * Ready-to-use application template
  * Complete integration example

### **API Specifications**

<figure><img src="../../../.gitbook/assets/截屏2025-07-29 15.06.45.png" alt=""><figcaption></figcaption></figure>

**Endpoint**

`GET https://<domain>/<serverpath>?address=<identifier>`

**Response Format**

`{ "result": { "point": 100 // Indicates task completion result } }`

**Important Notes**

* All API endpoints must be publicly accessible
* Optional bearer token support for TaskOn-exclusive access
* All identifiers are converted to **lowercase** for consistency
* Always return HTTP 200 status code
* Use `point` integer to indicate task completion result

**Example Request**

`GET <https://your-app.vercel.app/api/task/verification?address=0xd5045deea369d64ab7efab41ad18b82eeabcdefg`>

### **Task Configuration Steps** <a href="#task-configuration-steps" id="task-configuration-steps"></a>

**Slect API Task**

* Go to the TaskOn dashboard and click on the "API Task" tab.
* Click on the "Performance-Based Task" button.

<figure><img src="../../../.gitbook/assets/截屏2025-07-29 15.07.56.png" alt=""><figcaption></figcaption></figure>

#### **Fill in the Details**

* Complete all required fields & Upload the task icon.
* Click on the "Set API URL" button.

<figure><img src="../../../.gitbook/assets/截屏2025-07-29 15.08.43.png" alt=""><figcaption></figcaption></figure>

**Fill the api url**

* URL: If you use this repo and vercel, it shoud be like this: `https://xxx.vercel.app/api/task/verification`
* \[Optional] Bearer Token: Enable this to restrict API access to TaskOn only.

<figure><img src="../../../.gitbook/assets/截屏2025-07-29 15.10.01.png" alt=""><figcaption></figcaption></figure>

**Verify Configuration & Confirm Your Settings**

* **Purpose:** Ensure everything works smoothly.
* **Provide:** User ID that has points reward

After verification, it's all done.

<figure><img src="../../../.gitbook/assets/截屏2025-07-29 15.10.32.png" alt=""><figcaption></figcaption></figure>

### How it works <a href="#how-it-works" id="how-it-works"></a>

From the user side, users need to manually claim points for the first task completion. Afterward, points can be updated automatically via API when users click the refresh button.

View link:[**TaskOn API Verification Guide**](https://versed-catshark-f4d.notion.site/TaskOn-API-Verification-Guide-1f854c607cd349948c8db6f108fc39f1)
