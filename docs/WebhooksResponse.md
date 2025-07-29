# WebhooksResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Webhook]**](Webhook.md) |  | 
**included** | [**List[App]**](App.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhooks_response import WebhooksResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksResponse from a JSON string
webhooks_response_instance = WebhooksResponse.from_json(json)
# print the JSON string representation of the object
print(WebhooksResponse.to_json())

# convert the object into a dict
webhooks_response_dict = webhooks_response_instance.to_dict()
# create an instance of WebhooksResponse from a dict
webhooks_response_from_dict = WebhooksResponse.from_dict(webhooks_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


