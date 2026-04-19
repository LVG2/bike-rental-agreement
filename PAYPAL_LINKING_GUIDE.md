# How to Link Your PayPal Account - Step by Step

## 📋 What You Need:
- Your PayPal Business Account login
- Access to https://developer.paypal.com/

## 🔗 Step-by-Step Guide:

### Step 1: Log into PayPal Developer Portal
1. Visit: https://developer.paypal.com/
2. Click **Log In** (top right)
3. Use your PayPal account credentials

### Step 2: Find Your Client ID
1. On the left menu, click **Apps & Credentials**
2. Make sure you're on the **Sandbox** tab (for testing first)
3. Under "REST API apps" section:
   - If you see an app name (like "Default App"), click it
   - If not, create a new app by clicking "Create App"
4. You'll see your **Client ID** - this is a long string

**Example Client ID looks like:**
```
AaB3...r7M
```

### Step 3: Tell Me Your Client ID
Share your Client ID, and I'll update the HTML file to use it.

### Step 4: Test with Sandbox (Free!)
- Before going live, test with Sandbox:
  - Use test card: 4111 1111 1111 1111
  - Use any future expiration date
  - Use any CVV

### Step 5: Switch to Live (Production)
1. Go back to developer.paypal.com
2. Switch from **Sandbox** to **Production** tab
3. Get your Production Client ID
4. I'll update the HTML file with the production ID

## 🏦 For Bank Account Information:
If you want to add bank account fields for future use:
- Let me know and I can add a "Bank Information" section
- This would let customers optionally provide bank details

## ❓ Questions?
Reply with your Client ID (from Step 2) and I'll complete the setup!
