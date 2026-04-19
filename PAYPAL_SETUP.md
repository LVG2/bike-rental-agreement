# PayPal Integration Setup Guide

## Step 1: Create a PayPal Business Account
1. Go to https://www.paypal.com/business
2. Sign up for a Business account (if you don't have one)
3. Complete the verification process

## Step 2: Get API Credentials
1. Log into your PayPal Business account
2. Go to https://developer.paypal.com/
3. Create a new app or use existing one
4. Get your **Client ID** from the app settings

## Step 3: Configure the HTML File
1. Open `signing_document.html`
2. Find this line in the `<head>` section:
   ```html
   <script src="https://www.paypal.com/sdk/js?client-id=YOUR_PAYPAL_CLIENT_ID&components=buttons&currency=USD&intent=authorize"></script>
   ```
3. Replace `YOUR_PAYPAL_CLIENT_ID` with your actual Client ID from Step 2

## Step 4: Test the Integration
1. Open the HTML file in a web browser
2. Try the PayPal payment flow with a test payment
3. Complete the signature process

## Important Notes:
- The `intent=authorize` parameter ensures funds are **held** (not captured immediately)
- You can capture/void the authorization later through PayPal's dashboard or API
- For production use, you'll need to handle webhooks and server-side processing
- Test with PayPal's sandbox environment first: https://developer.paypal.com/tools/sandbox/

## Security Considerations:
- Never expose your Client ID in public repositories
- Use PayPal's sandbox for testing
- Implement proper error handling and user feedback
- Consider adding server-side verification of payment completion

## For Production Use:
You'll need a backend server to:
- Verify payment completion
- Store payment details securely
- Handle refunds/releases of held funds
- Send confirmation emails
- Process webhooks from PayPal