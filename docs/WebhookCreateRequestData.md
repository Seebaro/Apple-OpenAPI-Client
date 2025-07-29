# WebhookCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**WebhookCreateRequestDataAttributes**](WebhookCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.webhook_create_request_data import WebhookCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookCreateRequestData from a JSON string
webhook_create_request_data_instance = WebhookCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(WebhookCreateRequestData.to_json())

# convert the object into a dict
webhook_create_request_data_dict = webhook_create_request_data_instance.to_dict()
# create an instance of WebhookCreateRequestData from a dict
webhook_create_request_data_from_dict = WebhookCreateRequestData.from_dict(webhook_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


