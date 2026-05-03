

# WebhookPayloadLeadReceived

Webhook payload for the lead.received event. Fired when a Meta Lead Gen Form receives a new submission. Real-time delivery requires the page to be subscribed to the `leadgen` webhook field — Zernio subscribes on connect; existing accounts get backfilled by `scripts/backfill-fb-webhook-subscriptions.ts`.  Requires the Ads add-on. Subscribers without the add-on are filtered at delivery time. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Stable webhook event ID |  |
|**event** | [**EventEnum**](#EventEnum) |  |  |
|**lead** | [**Lead**](Lead.md) |  |  |
|**account** | [**WebhookPayloadLeadReceivedAccount**](WebhookPayloadLeadReceivedAccount.md) |  |  |
|**timestamp** | **OffsetDateTime** |  |  |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| LEAD_RECEIVED | &quot;lead.received&quot; |



