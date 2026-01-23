# Software-construction-mobile-app

App Chosen: WhatsApp

Part A: Understanding the App

1. App Overview
	•	What problem does this app solve?
WhatsApp solves the problem of fast, reliable and affordable communication between people regardless of distance over the internet.

WhatsApp is an alternative to traditional communication methods such as SMS and international phone calls are:
	 •	Expensive
	 •	Limited in features
	 •	Dependent on telecom networks rather than the internet

Who are the primary users of the app?
Friends, Families, Groups(students, communities, work teams) and Businesses.

3. Core Features
	•	Phone-based registeration and login 
	•	Text messaging and voice notes(1:1 chats and group chats)
	•	Voice and Video calls
	•	Media sharinh(Images, videos, documents)
	•	Status updates
	•	Notifications
 • Privacy and Security features such as end-to-end encryption, two-step verification, hiding last seen, profile picture and read receipts.

Part B: Thinking Behind the Scenes 

1. User Registration & Authentication
UI: Phone number input screens, OTP entry screen
Business Logic: User verification, session management
Network / APIs: SMS/OTP verification services, authentication servers
Data Storage: User profiles, device identifiers
Internet Required: Yes
If network is slow/unavailable: OTP delays, login failure

2. One-to-One Messaging
UI: Chat screen, message bubbles
Business Logic: Message formatting, encryption/decryption
Network / APIs: Message delivery servers
Data Storage: Message history (local + server backup metadata)
Internet Required: Yes (except viewing cached messages)
If network is slow/unavailable: Messages stay pending or unsent

3. Voice & Video Calls
UI: Call screens, call controls
Business Logic: Call setup, encryption, call state handling
Network / APIs: Real-time communication servers
Data Storage: Call logs (metadata only)
Internet Required: Yes (strong connection)
If network is slow/unavailable: Call drops, poor audio/video quality

4. Media Sharing
UI: Gallery picker, preview screens
Business Logic: Compression, encryption
Network / APIs: Media upload/download servers
Data Storage: Media files 
Internet Required: Yes
If network is slow/unavailable: Upload/download delays or failures

5. Notifications
UI: Notification banners, badges
Business Logic: Message prioritization
Network / APIs: Push notification services
Data Storage: Notification state
Internet Required: Yes
If network is slow/unavailable: Late or missing notifications

6. Status Updates
UI: Status viewer screen, progress indicators, privacy settings
Business Logic: Status expiration (24 hours), privacy controls (who can view)
Network / APIs: Media upload/download servers, contact synchronization services
Data Storage: Status media files, timestamps, viewer metadata
Internet Required: Yes
If network is slow/unavailable: Status uploads may fail, viewing may be delayed or unavailable

Part C: Change and Maintainability

Chosen Change:

1. Parts of the App That Would Need Changes
	•	Which components or layers of the app would be affected?

2. Existing Features That Could Break
	•	Which current features might be impacted by this change?

3. Why This Change Would Be Difficult
	•	What makes this change challenging from a software construction perspective?

Part D: Software Construction Challenges

Identify and briefly explain at least five engineering challenges involved in maintaining or improving this app:
	1.	
	2.	
	3.	
	4.	
	5.	

Part E: Group Reflection

1. Complexity 
	•	What surprised the group most about the complexity behind this app?

2. Software Quality 
	•	Why is writing “working code” not enough for software systems of this scale?

3. Teamwork 
	•	What did the group learn about teamwork from this exercise?

Group Contributions

