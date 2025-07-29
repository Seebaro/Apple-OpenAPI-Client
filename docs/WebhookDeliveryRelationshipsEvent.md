# WebhookDeliveryRelationshipsEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WebhookDeliveryRelationshipsEventData**](WebhookDeliveryRelationshipsEventData.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_delivery_relationships_event import WebhookDeliveryRelationshipsEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryRelationshipsEvent from a JSON string
webhook_delivery_relationships_event_instance = WebhookDeliveryRelationshipsEvent.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryRelationshipsEvent.to_json())

# convert the object into a dict
webhook_delivery_relationships_event_dict = webhook_delivery_relationships_event_instance.to_dict()
# create an instance of WebhookDeliveryRelationshipsEvent from a dict
webhook_delivery_relationships_event_from_dict = WebhookDeliveryRelationshipsEvent.from_dict(webhook_delivery_relationships_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


