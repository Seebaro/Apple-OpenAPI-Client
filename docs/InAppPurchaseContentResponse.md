# InAppPurchaseContentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseContent**](InAppPurchaseContent.md) |  | 
**included** | [**List[InAppPurchaseV2]**](InAppPurchaseV2.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_content_response import InAppPurchaseContentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseContentResponse from a JSON string
in_app_purchase_content_response_instance = InAppPurchaseContentResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseContentResponse.to_json())

# convert the object into a dict
in_app_purchase_content_response_dict = in_app_purchase_content_response_instance.to_dict()
# create an instance of InAppPurchaseContentResponse from a dict
in_app_purchase_content_response_from_dict = InAppPurchaseContentResponse.from_dict(in_app_purchase_content_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


