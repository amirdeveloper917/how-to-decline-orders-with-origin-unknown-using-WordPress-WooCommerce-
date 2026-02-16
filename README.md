# how-to-decline-orders-with-origin-unknown-using-WordPress-WooCommerce-
Blocks WooCommerce card testing attacks by enforcing a minimum order amount and validating suspicious checkout attribution before processing payment.


# WooCommerce Card Testing Protection

This lightweight snippet helps prevent card testing attacks on WooCommerce stores.

## What It Does

- Blocks checkout if order total is below a defined minimum amount
- Detects suspicious or missing order attribution
- Prevents fake / bot-driven card testing attempts
- Works without CAPTCHA

## Why This Is Needed

Card testing attacks typically:
- Use very small transaction amounts
- Trigger multiple failed orders
- Attempt random card numbers via checkout

This protection reduces gateway abuse and fraudulent activity.

## Installation

1. Add the code to your child theme `functions.php`
   OR
2. Create a small custom plugin and activate it.

## Recommended Setup

For stronger protection, combine this with:
- Authorize.Net AVS + CVV strict validation
- Checkout rate limiting (Cloudflare or server firewall)
- Minimum order threshold

## License

MIT
