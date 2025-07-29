# InAppPurchaseImageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseImageCreateRequestData**](InAppPurchaseImageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_image_create_request import InAppPurchaseImageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImageCreateRequest from a JSON string
in_app_purchase_image_create_request_instance = InAppPurchaseImageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImageCreateRequest.to_json())

# convert the object into a dict
in_app_purchase_image_create_request_dict = in_app_purchase_image_create_request_instance.to_dict()
# create an instance of InAppPurchaseImageCreateRequest from a dict
in_app_purchase_image_create_request_from_dict = InAppPurchaseImageCreateRequest.from_dict(in_app_purchase_image_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


