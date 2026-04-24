# Brave Browser Linux Debloat & Optimization Guide 

Brave is an excellent Chromium-based browser with a powerful built-in ad blocker (Shields). However, over time, it has accumulated unnecessary bloatware such as Crypto Wallets, BAT Rewards, and built-in AI (Leo). 

The goal of this guide is to completely Debloat the browser on Linux, returning it to a clean, minimal, and lightning-fast state, minimizing RAM usage, and maximizing privacy.

---

## 🛠️ Step 1: UI Cleanup (Visual Debloat)

First, we need to remove visual clutter and background scripts that consume bandwidth on the New Tab page.

### 1. New Tab Page
Open a new tab, scroll to the bottom right, and click on Customize:
- Background Image: Disable Show Sponsored Images to block background ads.
- Top Sites: Disable this to clean up the center of the screen.
- Cards: Disable completely.
- Brave News: Turn this off entirely to prevent unnecessary background bandwidth usage.

### 2. Address Bar & Sidebar (Appearance)
Go to Settings > Appearance:
- Hide Annoying Icons: Disable the following options:
  - Show Brave Rewards button (Hides the red triangle).
  - Show Brave Wallet icon.
  - Show VPN button.
  - Show Leo AI button.
- Sidebar: Find Show Sidebar and set it to Never.

---

## 🛡️ Step 2: Shields & Privacy Settings

This is the core strength of Brave. Configuring this correctly eliminates the need for third-party extensions like uBlock Origin.

### 1. Blocking Power
Go to Settings > Shields:
- Set Trackers & ads blocking to Aggressive.

### 2. Content Filtering
In the same Shields menu, scroll down and click on Content Filtering. 
*(Note: Do not enable all filters as it may break websites. Enable only what you need).*
Recommended filters:
- Fanboy's Annoyances and uBO Annoyances (Hides cookie consent pop-ups and annoying elements).
- Arabic website ad blocker - Liste AR (Crucial for blocking malicious ads on Arabic sites).
- YouTube filters (Optional: to hide Shorts or recommendations).

### 3. Disable Telemetry
Go to Settings > Privacy and security > Data collection:
- Disable Allow privacy-preserving product analytics.
- Disable Automatically send daily usage ping to Brave.

---

## ⚙️ Step 3: Disable Web3 & AI Services

Since we do not need the Crypto Wallet or the built-in AI assistant:
- Web3: Go to settings and set all Web3 domains/features to Disabled.
- Leo AI: Ensure all AI suggestions and autocomplete features are turned off to prevent sending search queries to external servers.

---

## 🚀 Step 4: Performance & RAM Optimization

To reduce the RAM consumption of the Chromium engine on Linux:
- Go to Settings > System:
  - Disable Continue running background apps when Brave is closed (Ensures Brave closes completely and frees RAM).
  - Enable Use graphics acceleration when available (Offloads UI rendering and video decoding to the GPU).
- Memory Saver: Enable this feature. The browser will automatically freeze inactive tabs to save system resources.

---

## 🔑 Step 5: Password Management (Security)

Storing passwords inside the browser is a bad security practice.
- Go to Settings > Autofill and passwords > Password Manager:
  - Disable Offer to save passwords.
  - Disable Auto Sign-in.
- Recommended Alternative: Use a dedicated, open-source password manager like Bitwarden or KeePassXC.

---

## 🔧 Step 6: Troubleshooting

Because we set the Shields to "Aggressive", you might encounter broken websites or connection issues (e.g., speed test tools like fast.com or payment gateways). 

How to fix this quickly:

1. The Quick Fix (Shields Down):
   - Click the Brave Lion icon in the address bar.
   - Toggle the Shields to DOWN for that specific site. It will reload and work normally.
