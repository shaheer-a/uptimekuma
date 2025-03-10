# Uptime Kuma Monitor Configuration

This guide provides step-by-step instructions to configure an **HTTP(s) Monitor** in **Uptime Kuma** for monitoring.

## **Monitor Details**

| Parameter | Value |
|-----------|-------|
| **Monitor Type** | HTTP(s) |
| **Friendly Name** | Example-App |
| **URL** | [https://example-app.com |
| **Heartbeat Interval** | 60 seconds |
| **Retries** | 0 |
| **Heartbeat Retry Interval** | 60 seconds |
| **Request Timeout** | 48 seconds |
| **Resend Notification if Down X times consecutively** | 0 (Disabled) |

## **Advanced Settings**

| Parameter | Value |
|-----------|-------|
| **Certificate Expiry Notification** | Enabled |
| **Ignore TLS/SSL Errors** | Disabled |
| **Upside Down Mode** | Disabled |
| **Max. Redirects** | 10 |
| **Accepted Status Codes** | 200-299 |

## **Monitor Group**
- No group assigned. Create a Group Monitor first if needed.

## **Tags & Description**
- No tags or description added. You can customize these based on your needs.

## **Setup Instructions**
1. **Log in** to your **Uptime Kuma** instance.
2. Click on **"Add New Monitor"**.
3. Select **"HTTP(s)"** as the monitor type.
4. Enter the **Friendly Name** as **Example-App**.
5. Set the **URL** to **https://example-app.com**.
6. Configure the **Heartbeat Interval** to **60 seconds**.
7. Set **Retries** to **0**.
8. Configure **Heartbeat Retry Interval** to **60 seconds**.
9. Set **Request Timeout** to **48 seconds**.
10. Disable **Resend Notification if Down** (set to **0**).
11. In the **Advanced Settings**:
    - Enable **Certificate Expiry Notification**.
    - Set **Max. Redirects** to **10**.
    - Ensure **Accepted Status Codes** is **200-299**.
12. Click **Save** to create the monitor.

---

# Uptime Kuma Slack Notification Configuration

This guide provides step-by-step instructions to configure a **Slack Notification** in **Uptime Kuma** for monitoring.

## **Notification Details**

| Parameter | Value |
|-----------|-------|
| **Notification Type** | Slack |
| **Friendly Name** | Example-App |
| **Webhook URL** | your-slack-webhook-url |
| **Username** | _(Optional)_ |
| **Icon Emoji** | _(Optional)_ |
| **Channel Name** | `example-app` |
| **Notify Channel** | Enabled |
| **Apply on all existing monitors** | Enabled |

## **Setup Instructions**
1. **Log in** to your **Uptime Kuma** instance.
2. Navigate to **Settings > Notification** and click **"Setup Notification"**.
3. Select **Slack** as the notification type.
4. Enter the **Friendly Name** as **Example-App**.
5. Paste the **Webhook URL**:  
   `https://hooks.slack.com/services/xyz`
6. (Optional) Set a **Username** for the notification.
7. (Optional) Choose an **Icon Emoji**.
8. Enter the **Channel Name** as **example-app**.
9. Ensure **Notify Channel** is **Enabled** (this ensures notifications reach all members).
10. Enable **Apply on all existing monitors** if you want this notification to apply across all monitors.
11. Click **Save** to apply the settings.

