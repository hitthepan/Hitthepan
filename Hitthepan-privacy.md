# Privacy Policy

**Last Updated: March 30, 2026**

**Effective Date: March 30, 2026**

Hasan Balki ("we," "our," or "us") operates HitThePan (the "App"), a beauty product tracking application available on Apple's App Store. This Privacy Policy is available at https://hitthepan.github.io/Hitthepan/privacy.md. Your use of the App is also governed by our Terms of Service, available at https://hitthepan.github.io/Hitthepan/terms.md.

This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use the App. By downloading, installing, or using the App, you agree to the collection and use of information in accordance with this Privacy Policy. If you do not agree with the terms of this Privacy Policy, please do not access or use the App.

---

## 1. Information We Collect

### 1.1 Information You Provide Directly

**Account Information**
- Display name
- Email address (provided through Apple Sign-In or Google Sign-In)
- Username (optional, for social features)
- Profile avatar photo (optional)

**Product Data**
- Product names, brands, categories, and shades
- Usage counts and tracking goals
- Purchase dates and prices
- Product photos (optional)
- Repurchase verdicts

**Financial Tracking Data**
- Saved purchase records (product name, brand, amount, reason)
- Dream reward goals (name, target amount)

**Diary Entries**
- Text notes associated with products
- Diary photos

**Routine Data**
- Custom routine names and associated products

**Social Interactions**
- Friend requests and connections
- User reports (including reason text)
- Block actions

### 1.2 Information Collected Automatically

**Analytics Data (With Your Consent)**
- App usage events (e.g., screens viewed, features used, products added)
- Device type and operating system version
- App version
- Subscription status (premium or free)

**Crash and Performance Data (With Your Consent)**
- Crash reports including stack traces
- App performance metrics
- Error context information

**Device Identifiers**
- Unique user identifier (UUID) generated at account creation
- No advertising identifiers are collected

### 1.3 Information We Do NOT Collect

- We do not collect precise geolocation data
- We do not collect contacts or address book data
- We do not collect browsing history
- We do not collect health or fitness data
- We do not collect financial or payment card information (all payments are processed by Apple through the App Store)
- We do not use advertising identifiers or track users across apps

---

## 2. How We Use Your Information

We use the information we collect for the following purposes:

| Purpose | Legal Basis (GDPR) |
|---------|-------------------|
| Provide and maintain the App's core functionality | Performance of contract |
| Create and manage your account | Performance of contract |
| Sync your data across sessions | Performance of contract |
| Process subscription purchases (via Apple) | Performance of contract |
| Enable social features (friends, leaderboard) | Performance of contract |
| Send local notification reminders (with permission) | Consent |
| Analyze app usage to improve features | Consent |
| Diagnose crashes and fix bugs | Consent |
| Respond to user reports and enforce community standards | Legitimate interest |
| Comply with legal obligations | Legal obligation |

---

## 3. Third-Party Services

We use the following third-party services to operate the App:

### 3.1 Supabase (Database & Authentication)

- **Purpose:** Cloud database, user authentication, and real-time data synchronization  
- **Data processed:** All user-generated content, account information, social connections  
- **Data location:** Supabase infrastructure (AWS)  
- **Privacy policy:** https://supabase.com/privacy  

### 3.2 Firebase by Google

**Firebase Analytics**
- **Purpose:** Anonymous app usage analytics (only with your consent)  
- **Data processed:** Usage events, screen views, device type, app version  
- **Data retention:** 14 months (Google default)  
- **Privacy policy:** https://firebase.google.com/support/privacy  

**Firebase Crashlytics**
- **Purpose:** Crash reporting and stability monitoring (only with your consent)  
- **Data processed:** Crash logs, stack traces, device information, user ID, subscription status  
- **Data retention:** 90 days  

**Firebase Remote Config**
- **Purpose:** Feature configuration and A/B testing  
- **Data processed:** Device metadata for targeting (no personal data)  

### 3.3 RevenueCat

- **Purpose:** Subscription management and entitlement verification  
- **Data processed:** User identifier, subscription status, purchase events  
- **Data location:** RevenueCat infrastructure  
- **Privacy policy:** https://www.revenuecat.com/privacy  

### 3.4 Apple Sign-In

- **Purpose:** User authentication  
- **Data processed:** Name, email address (may be relayed/hidden per user preference)  
- **Privacy policy:** https://www.apple.com/legal/privacy/  

### 3.5 Google Sign-In

- **Purpose:** User authentication  
- **Data processed:** Name, email address, profile identifier  
- **Privacy policy:** https://policies.google.com/privacy  

### 3.6 Open Beauty Facts

- **Purpose:** Product barcode lookup (optional feature)  
- **Data processed:** Barcode numbers only; no personal data is sent  
- **Privacy policy:** https://world.openbeautyfacts.org/terms-of-use  

---

## 4. Data Storage and Security

### 4.1 Where Your Data Is Stored

| Storage Location | Data Types | Encryption |
|-----------------|------------|------------|
| Supabase (Cloud) | Account data, products, usage logs, diary text, social data, purchases, dreams, badges, routines | Encrypted in transit (TLS) and at rest |
| Device — CoreData | Diary photos and thumbnails | iOS file protection (NSFileProtectionComplete) |
| Device — File System | Product images, dream images, avatar photo | iOS file protection |
| Device — Keychain | Authentication tokens, user ID | iOS Keychain encryption (hardware-backed) |
| Device — UserDefaults | Preferences (dark mode, reminders, consent) | Standard iOS protection |

### 4.2 Security Measures

- All network communication uses HTTPS/TLS encryption  
- Authentication tokens are stored in the iOS Keychain with `.whenUnlockedThisDeviceOnly` accessibility  
- Local database files use iOS file protection (complete encryption when device is locked)  
- Row-Level Security (RLS) policies ensure users can only access their own data on our backend  
- API rate limiting prevents abuse (120 requests/minute general, 30 requests/minute for write operations)  
- A privacy screen (blur overlay) is applied when the app moves to the background to protect visible content  

### 4.3 Data Retention

- **Account data:** Retained until you delete your account  
- **Product and usage data:** Retained until you delete the specific item or your account  
- **Analytics data:** 14 months (Firebase default), collected only with your consent  
- **Crash reports:** 90 days (Firebase Crashlytics default), collected only with your consent  
- **User reports:** Retained for up to 2 years from the date of submission, or longer if required for ongoing investigations or legal proceedings  
- **Temporary export files:** Deleted automatically after download  

---

## 11. Supplementary Technical Information

### 11.1 API Usage Declarations

As required by Apple, the App declares usage of the following system APIs in its privacy manifest:
- **UserDefaults** — For storing user preferences and app settings  
- **File Timestamp** — For managing cached files  
- **Disk Space** — For ensuring sufficient storage before saving photos  

### 11.2 Encryption

The App does not use non-exempt encryption. All encryption is provided by standard iOS frameworks (HTTPS/TLS) and third-party services.

### 11.3 Tracking

The App does not track users across other companies' apps or websites. `NSPrivacyTracking` is set to `false` in our privacy manifest. No advertising identifiers (IDFA) are collected.