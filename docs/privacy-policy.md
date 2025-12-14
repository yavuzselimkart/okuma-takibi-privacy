# 📄 Reading Tracker – Privacy Policy

**Last Updated:** December 14, 2025

This Privacy Policy explains how Reading Tracker (“the App”) processes, stores, and protects user information.  
By using the App, you agree to this Privacy Policy.

---

## 📍 1. Permissions and Their Use

The App only uses permissions that are strictly necessary for its core functionality:

### 1.1 Camera Permission
- The camera permission is used **only when the user explicitly initiates taking a photo**.
- The camera is **never accessed in the background** or without user interaction.

### 1.2 Gallery / Photo Selection
- Selecting images from the gallery is done via the **Android System Photo Picker**.
- The App does **not request broad or persistent access** to the user’s entire photo or video library.
- Only images explicitly selected by the user are accessed.

### 1.3 Advertising ID (AD_ID)
- The App uses **Google Mobile Ads (AdMob)**.
- The Advertising ID (AD_ID) is used to serve personalized or non-personalized ads.
- Ad-related data is processed in accordance with Google’s own privacy policy.

**AdMob Privacy Policy:**  
https://policies.google.com/privacy

---

## 🖼️ 2. Data Collected and How It Is Used

### 2.1 Cover Image (Photo)
- The book cover image taken or selected by the user is stored **locally on the device**.
- To extract book information such as **title, author, and page count**, the **base64-encoded content** of the image is sent over an encrypted connection (HTTPS/TLS) to the following endpoint:

```

[https://api.readingtracker.yazilimkodu.com/api/chat/ask](https://api.readingtracker.yazilimkodu.com/api/chat/ask)

```

- The image is used solely for this purpose and is **not used for marketing or advertising**.

### 2.2 Anonymous Device Identifier (UUID)
- To limit requests and prevent abuse, the App generates an **anonymous UUID** that is stored locally on the device (via SharedPreferences).
- This identifier is sent in the request headers when communicating with the server.
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

---

## 🔒 3. Data Storage and Deletion

- Images and app data are stored **only on the user’s device**, within the app’s local storage.
- When the App is uninstalled, **all local data is automatically deleted**.
- Currently, the App does **not** include:
  - Cloud backups
  - User accounts
  - Server-side persistent storage

If such features are added in the future, this Privacy Policy will be updated accordingly.

---

## 🔁 4. Data Sharing

The App:
- Does **not sell, rent, or share** personal data for marketing purposes.

Data may be shared **only for the following limited purposes**:

1. **Cover Extraction API**
   - Shared data: Cover image (base64) + anonymous device UUID
   - Purpose: Book information extraction

2. **Google Mobile Ads (AdMob)**
   - Shared data: Advertising-related data
   - Purpose: Ad display

---

## 🛡️ 5. Security

- All server communication is protected using **TLS / HTTPS**.
- Technical measures are taken to prevent unauthorized access and misuse.
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
