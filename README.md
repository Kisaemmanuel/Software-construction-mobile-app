# Software-Construction-Mobile-App: WhatsApp

## Part A: Understanding the App

### 1. App Overview

#### What problem does the app solve?
WhatsApp solves the problem of **fast, reliable, and affordable communication** between people regardless of distance by using the internet instead of traditional telecom networks.

It serves as an alternative to traditional communication methods such as **SMS and international phone calls**, which are often:
- Expensive
- Limited in features
- Dependent on mobile network providers rather than the internet

By using internet connectivity, WhatsApp enables real-time messaging, calling, and media sharing at a much lower cost.

#### Who are the primary users of the app?
The primary users of WhatsApp include:
- Friends and families
- Groups such as students, communities, and work teams
- Small and medium-sized businesses communicating with customers


### 2. Core Features
Key features provided by WhatsApp include:
- Phone number–based registration and user authentication
- Text messaging and voice notes (one-to-one chats and group chats)
- Voice and video calling
- Media sharing (images, videos, and documents)
- Status updates for sharing temporary content
- Push notifications for new messages and calls
- Privacy and security features such as:
  - End-to-end encryption
  - Two-step verification
  - Privacy controls (e.g., hiding last seen and profile visibility)

---


## Part B: Thinking Behind the Scenes

This section explains what happens behind the scenes for key WhatsApp features, focusing on UI, logic, networking, and data handling.

### 1. User Registration & Authentication
- **UI:** Phone number input screens, OTP entry screen  
- **Business Logic:** User verification, OTP validation, session management  
- **Network / APIs:** SMS/OTP verification services, authentication servers  
- **Data Storage:** User profiles, device identifiers  
- **Internet Required:** Yes  
- **If network is slow/unavailable:** OTP delays, login failure  

### 2. One-to-One Messaging
- **UI:** Chat screen, message bubbles  
- **Business Logic:** Message formatting, end-to-end encryption/decryption  
- **Network / APIs:** Message delivery servers  
- **Data Storage:** Message history (local storage and server backup metadata)  
- **Internet Required:** Yes (except for viewing cached messages)  
- **If network is slow/unavailable:** Messages remain pending or unsent  

### 3. Voice & Video Calls
- **UI:** Call screens, call controls (mute, speaker, video)  
- **Business Logic:** Call setup, encryption, call state handling  
- **Network / APIs:** Real-time communication servers  
- **Data Storage:** Call logs  
- **Internet Required:** Yes (strong and stable connection)  
- **If network is slow/unavailable:** Call drops, poor audio/video quality  

### 4. Media Sharing
- **UI:** Gallery picker, preview screens  
- **Business Logic:** Media compression, encryption  
- **Network / APIs:** Media upload and download servers  
- **Data Storage:** Media files (stored locally and in backups)  
- **Internet Required:** Yes  
- **If network is slow/unavailable:** Upload/download delays or fails to be delivered  

### 5. Notifications
- **UI:** Notification banners, icons, badges  
- **Business Logic:** Message prioritization and notification triggers  
- **Network / APIs:** Push notification services  
- **Data Storage:** Notification state and delivery status  
- **Internet Required:** Yes  
- **If network is slow/unavailable:** Late or missing notifications  

### 6. Status Updates
- **UI:** Status viewer screen, progress indicators, privacy settings  
- **Business Logic:** Status expiration after 24 hours, visibility controls  
- **Network / APIs:** Media upload/download servers, contact synchronization services  
- **Data Storage:** Status media files, timestamps, viewer metadata  
- **Internet Required:** Yes  
- **If network is slow/unavailable:** Status upload failures or delayed viewing(blur images)  

### 7. Privacy & Security Features
- **UI:** Security notifications, encryption information screens, privacy settings  
- **Business Logic:** End-to-end encryption, access control rules, message decryption on devices  
- **Network / APIs:** Secure message relay servers (cannot read message content)  
- **Data Storage:** Encrypted messages stored on user devices  
- **Internet Required:** Yes   
- **If network is slow/unavailable:** Messages are queued and sent when connectivity is restored
  
---
## Part C: Change and Maintainability

### Chosen Change Scenario: Add Mobile Payments in Uganda

This change involves adding a feature that allows WhatsApp users in Uganda to send and receive money using local mobile money services such as MTN Mobile Money and Airtel Money.

---

### 1. Which parts of the app would need changes?

**User Interface (UI):**  
- Add a “Send Money” option within chats  
- Screens for entering amount, confirming payment, and viewing transaction history  
- Clear success and error messages for payment status  

**Business Logic:**  
- Rules for sending and receiving money  
- Transaction limits and validation  
- Handling pending, failed, and reversed payments  

**Network / APIs:**  
- Integration with mobile money service providers  
- Real-time communication to verify payment transactions  

**Data Storage:**  
- Secure storage of transaction records  
- Audit logs for tracking and dispute resolution  

**Security Systems:**  
- PIN or biometric authentication  
- Fraud detection mechanisms and strong encryption  

---

### 2. What existing features could break?

- Chat performance may slow down if payment processing affects messaging flow  
- Poor network conditions may cause delayed or unclear payment confirmations  
- Notifications may be delayed or duplicated, confusing users  
- Increased security risks may expose the app to fraud or attacks  
- User trust may be affected if payments fail or behave inconsistently  

---

### 3. Why would this change be difficult to implement?

- WhatsApp was originally designed for messaging, not financial transactions  
- Payments require extremely high reliability compared to normal messages  
- Integration with local mobile money providers adds technical complexity  
- Compliance with financial regulations is required  
- Unstable internet connections make payment confirmation challenging  

---

### Summary

Adding mobile payments in Uganda is a complex change because it requires major updates to the user interface, backend systems, security, and external integrations, while ensuring reliability, regulatory compliance, and user trust.

## Part D: Software Construction Challenges

Identify and briefly explain at least five engineering challenges involved in maintaining or improving this app:

1.Scalability
A WhatsApp-like app must support millions of users sending messages simultaneously. Designing systems that scale without delays or crashes is a major engineering challenge.
2.Real-time Communication
Ensuring messages are delivered instantly requires reliable real-time protocols, stable network connections, and efficient handling of message synchronization across devices.
Security and Privacy
3.Implementing end-to-end encryption to protect user messages while still maintaining performance and usability is complex and requires careful design and testing.
4.Maintainability and Code Complexity
As features like voice calls, video calls, status updates, and group chats are added, the codebase becomes large and complex, making it harder to maintain and update without introducing bugs.
5.Cross-Platform Compatibility
The app must work consistently across different devices and operating systems (Android, iOS, web). Ensuring the same user experience and behavior on all platforms is challenging.
## Part E:  Group Reflection

1. Complexity 
	•	What surprised the group most about the complexity behind this app?

2. Software Quality 
	•	Why is writing “working code” not enough for software systems of this scale?

3. Teamwork 
	•	What did the group learn about teamwork from this exercise?

## Group Contributions
- KISA EMMANUEL: Coordination and app overview
- NICOLE JOHNSON: Feature analysis
- NANKYA ZAHARA: Backend and system reasoning
- ARIKO ETHAN: Change and risk analysis
- KISA EMMANUEL: Documentation and final review


