---
meta:
  - name: description
    content: Linking Snipcart and Craft CMS with webhooks.
---

# Linking Snipcart and Craft

Get your webhook endpoint from the _Webhooks_ tab in the plugin settings:

![Craft's webhook endpoint](../../resources/settings-webhooks.png)

Add it to the _Webhooks URL_ field in [Snipcart's control panel](https://app.snipcart.com/):

![Snipcart webhook setting](../../resources/snipcart-webhook.png)

That's it! Now Snipcart will post data to your Craft site as stuff happens with the store. Live webhooks will automatically be [secured and validated](https://docs.snipcart.com/v2/webhooks/introduction#secure-your-webhook-endpoint), and when `devMode` is enabled _all_ webhook posts will be allowed through.

Webhook transactions are logged under _Requests History_ in the Snipcart control panel, so you can confirm success or investigate problems there.