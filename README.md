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

## Part C: Change and Maininability
Chosen Change:

1. Parts of the App That Would Need Changes
	•	Which components or layers of the app would be affected?

2. Existing Features That Could Break
	•	Which current features might be impacted by this change?

3. Why This Change Would Be Difficult
	•	What makes this change challenging from a software construction perspective?

---


## Part D: Software Construction Challenges

Identify and briefly explain at least five engineering challenges involved in maintaining or improving this app:
	1.	
	2.	
	3.	
	4.	
	5.	

---

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


