# WebhookDeliveryRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event** | [**WebhookDeliveryRelationshipsEvent**](WebhookDeliveryRelationshipsEvent.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_delivery_relationships import WebhookDeliveryRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryRelationships from a JSON string
webhook_delivery_relationships_instance = WebhookDeliveryRelationships.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryRelationships.to_json())

# convert the object into a dict
webhook_delivery_relationships_dict = webhook_delivery_relationships_instance.to_dict()
# create an instance of WebhookDeliveryRelationships from a dict
webhook_delivery_relationships_from_dict = WebhookDeliveryRelationships.from_dict(webhook_delivery_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


