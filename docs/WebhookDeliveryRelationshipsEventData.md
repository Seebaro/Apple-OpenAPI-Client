# WebhookDeliveryRelationshipsEventData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 

## Example

```python
from openapi_client.models.webhook_delivery_relationships_event_data import WebhookDeliveryRelationshipsEventData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryRelationshipsEventData from a JSON string
webhook_delivery_relationships_event_data_instance = WebhookDeliveryRelationshipsEventData.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryRelationshipsEventData.to_json())

# convert the object into a dict
webhook_delivery_relationships_event_data_dict = webhook_delivery_relationships_event_data_instance.to_dict()
# create an instance of WebhookDeliveryRelationshipsEventData from a dict
webhook_delivery_relationships_event_data_from_dict = WebhookDeliveryRelationshipsEventData.from_dict(webhook_delivery_relationships_event_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


