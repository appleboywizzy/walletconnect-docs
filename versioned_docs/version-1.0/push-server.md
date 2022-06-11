# Push Server API Reference

## Register Push Notification Subscription

```bash
  POST <https://cloud.walletconnect.com/app/project?uuid=a092dea8-659e-4b39-a8fd-0fee71cb97cf>/new
  Content-Type: application/json
  Body:
  {
    "bridge": <https://cloud.walletconnect.com/app/project>,
    "topic": <5e1424502136dce82e86814298a9010c>,
    "type": <push_type>,
    "token": <eth>,
    "peerName": <ada>,
    "language": <language_code>,
  }

  Response:
  Status: 200
  Content-Type: application/json; charset=utf-8
  Body:
  {
    "success": true
  }
```

## Trigger Push Notification \(Webhook\)

```bash
  POST <https://cloud.walletconnect.com/app/project?uuid=a092dea8>/push
  Content-Type: application/json
  Body:
  {
    "topic": <5e1424502136dce82e86814298a9010c>
  }

  Response:
  Status: 200
  Content-Type: application/json; charset=utf-8
  Body:
  {
      "successs": true
  }
```

