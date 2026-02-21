---
title: Privacy Policy
permalink: /privacy/
---


# Privacy Policy

**Last Updated: February 21, 2026**

Jomood ("we," "our," or "us") is a local-first mood journaling app. This Privacy Policy explains what data is processed, when it leaves your device, and which third-party services/libraries are involved.

## 1. Local-First Data Model

By default, your journal data stays on your device.

- Journal entries, tags, moods, media metadata, and AI outputs are stored locally.
- Photos/videos attached to entries are stored on your device.
- Location coordinates are stored locally only if you choose to attach location.
- Security settings (such as PIN lock state) are stored locally; PIN values are hashed before storage.

## 2. Data We Process

### 2.1 AI Features (Reflect Chat and Periodic Reviews)

If you use AI features, we send only the content needed to generate that response.

- Data sent: entry text, mood/emotion/theme context, language, and conversation context.
- Transport path: app -> Firebase Cloud Functions -> Google Vertex AI (Gemini model).
- Authentication: anonymous Firebase Authentication token for callable functions.
- Retention: functions are stateless and do not intentionally persist entry content after processing.
- Local storage: generated AI messages/summaries are stored on your device.

### 2.2 Voice Input

When you use voice input, your device OS speech-recognition service processes microphone audio for transcription. Depending on platform/device settings, speech recognition may run on-device and/or via Apple/Google speech services. Jomood receives the transcribed text and uses it like typed input.

### 2.3 Cloud Backup (Google Drive, Optional)

If enabled by you:

- Google sign-in is used to authorize backup access.
- Backup files are uploaded to your Google Drive `appDataFolder`.
- We keep up to 3 most recent backups through app logic.
- Your backup files remain under your Google account control.

### 2.4 Analytics (Optional Consent)

If you opt in, Firebase Analytics collects usage telemetry (for example: feature usage, device/OS/app version, and AI feature event counts). You can withdraw consent in Settings.

### 2.5 Subscriptions

Subscriptions are sold through Apple App Store or Google Play. We use RevenueCat to manage entitlement status. We do not receive full payment card details.

## 3. Permissions We Request

Depending on feature usage and platform, Jomood may request:

- Camera/photo library access (attach or save media).
- Location access (tag entries with location and map features).
- Microphone/speech access (voice input).
- Notification permission (reminders and review notifications).
- Biometric auth permission (optional app lock).

Permissions are optional except where required for a specific feature.

## 4. Third-Party Services

| Service | Purpose | Typical Data |
|---|---|---|
| Firebase (Core/Auth/Functions/Analytics) | App infrastructure, anonymous auth for AI calls, optional analytics | Device/app identifiers, callable payloads for AI, optional analytics events |
| Google Vertex AI (Gemini) | AI response generation | Journal context sent for AI prompts |
| Google Sign-In + Google Drive API | Optional cloud backup | Google account auth data, backup files in your Drive app-data space |
| Google Maps Platform | Map display and map interactions | Map tile/API requests and approximate map-related metadata |
| RevenueCat | Subscription entitlement management | Subscription status and SDK identifiers |
| Apple App Store / Google Play Billing | Payment processing | Store-managed purchase transaction data |
| OS speech services (Apple/Google) | Speech-to-text for voice input | Microphone audio for transcription when voice input is active |

## 5. Retention and Deletion

- Local app data: kept until you delete entries, clear app data, or uninstall.
- Drive backups: kept until deleted from your Google Drive (or rotated by app logic).
- Analytics data: retained under Google/Firebase retention controls when consent is enabled.

## 6. International Processing

Third-party providers may process data on infrastructure outside your country. By using cloud features, you acknowledge such transfers may occur under provider terms.

## 7. Your Rights and Choices

- Disable analytics consent in app settings.
- Stop using AI features at any time.
- Delete local entries and media from your device.
- Remove backups from Google Drive.
- Contact us for privacy requests.

## 8. Security

- Network requests use HTTPS/TLS.
- Sensitive local secrets are stored with platform secure storage.
- Optional app lock supports PIN/biometric gating.

No system is 100% secure, but we implement reasonable safeguards.

## 9. Children

Jomood is not intended for children under 13. If you believe a child submitted personal data, contact us and we will help address it.

## 10. Changes to This Policy

We may update this policy. Material changes will be reflected by updating the "Last Updated" date and, when appropriate, in-app notice.

## 11. Contact

Email: **jomood.app@gmail.com**

