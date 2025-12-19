# 📄 Reading Tracker – Privacy Policy

**Last Updated:** December 14, 2025

This Privacy Policy explains how Reading Tracker (“the App”) processes, stores, and protects user information.  
By using the App, you agree to this Privacy Policy.

---

## 📍 1. Permissions and Their Use

The App only uses permissions that are strictly necessary for its core functionality.

### 1.1 Camera Permission
- The camera permission is used **only when the user explicitly initiates taking a photo**.
- The camera is **never accessed in the background** or without user interaction.

### 1.2 Gallery / Photo Selection
- Selecting images from the gallery is performed via the **Android System Photo Picker**.
- The App does **not request READ_MEDIA_\*** permissions and does **not request broad or persistent access** to the user’s entire photo or video library.
- Only images explicitly selected by the user are accessed.

### 1.3 Advertising ID (AD_ID)
- The App uses **Google Mobile Ads (AdMob)**.
- The Advertising ID (AD_ID) is used to serve personalized or non-personalized ads.
- Ad-related data is processed in accordance with Google’s own privacy policy.

**AdMob Privacy Policy:**  
https://policies.google.com/privacy

### 1.4 Notification Permission (Android 13+)
- On devices running **Android 13 (API level 33) or higher**, the App may request the **POST_NOTIFICATIONS** permission.
- This permission is used **only to display local (on-device) notifications** related to reading goals.
- Notifications are:
  - Fully optional and configurable by the user
  - Not used for advertising or marketing
  - Not used to track users
- The App does **not** send remote or server-based push notifications.

---

## 🖼️ 2. Data Collected and How It Is Used

### 2.1 Cover Image (Photo)
- The book cover image taken or selected by the user is stored **locally on the device**.
- To extract book information such as **title, author, and page count**, the **base64-encoded content** of the cover image is sent over an encrypted connection (HTTPS/TLS) to the following endpoint:

https://api.readingtracker.yazilimkodu.com/api/chat/ask

- The image is used solely for this purpose and is **not used for marketing or advertising**.

### 2.2 Anonymous Device Identifier (UUID)
- To limit requests and prevent abuse, the App generates an **anonymous UUID** that is stored locally on the device using **SharedPreferences**.
- This UUID is sent to the API **in the request headers** when communicating with the server.
- The UUID:
  - Does not contain personal data
  - Does not directly identify the user
  - Is not used for advertising or marketing purposes

### 2.3 Advertising Data
- Google Mobile Ads SDK (AdMob) may process:
  - Advertising ID
  - Device information
  - Approximate location and interaction signals  
  in accordance with its own policies.

### 2.4 Local Reading Goal Notifications
- The App may generate **local notifications** to support daily reading goals.
- Notification behavior is fully controlled by the user and may include:
  - Customizable time ranges
  - Notification frequency settings
  - A daily maximum notification limit
- Notifications automatically **stop once the daily reading goal is reached**.
- When a daily goal is completed, the App may display a confirmation message such as:  
  **“You’ve reached today’s goal.”**
- All notification logic runs **entirely on the device**.
- No notification-related data is sent to external servers.

---

## 🔒 3. Data Storage and Deletion

- Images, notification settings, and app-related data are stored **only on the user’s device**, within the app’s local storage.
- When the App is uninstalled, **all locally stored images, preferences, and data are automatically deleted**.
- Currently, the App does **not** include:
  - Cloud backups
  - User accounts
  - Server-side persistent storage

If such features are added in the future, this Privacy Policy will be updated accordingly.

---

## 🔁 4. Data Sharing

The App:
- Does **not sell or share data for marketing or advertising purposes**.

Data is shared **only in a limited and purpose-bound manner** with the following services:

1. **Cover Extraction API**
   - Shared data: Base64-encoded cover image + anonymous device UUID
   - Purpose: Book information extraction

2. **Google Mobile Ads (AdMob)**
   - Shared data: Advertising-related data
   - Purpose: Ad display

---

## 🛡️ 5. Security

- All communication with servers is protected using **TLS / HTTPS**.
- Technical and organizational measures are implemented to prevent unauthorized access and misuse.
- Users may contact us via email to exercise their data protection rights.

---

## 👶 6. Children’s Privacy

- The App is **not intended for children under the age of 13**.
- No personal data is knowingly collected from children under 13.
- If such data is identified, it will be deleted immediately.

---

## 🌍 7. International Use and User Rights

The App is available globally.  
Depending on their location, users may have rights under applicable data protection laws, including:

- Access to their data
- Requesting deletion of data
- Objecting to data processing  

(e.g. GDPR, KVKK, and similar regulations)

---

## 📬 8. Contact

For any questions or requests regarding this Privacy Policy:

**Email:** y.selimkart@gmail.com

---

## ✏️ 9. Changes

This Privacy Policy may be updated from time to time.  
Any changes take effect once published on this page.  
The latest update date is always shown at the top of this document.
