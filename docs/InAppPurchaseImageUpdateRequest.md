# InAppPurchaseImageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseImageUpdateRequestData**](InAppPurchaseImageUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_image_update_request import InAppPurchaseImageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImageUpdateRequest from a JSON string
in_app_purchase_image_update_request_instance = InAppPurchaseImageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImageUpdateRequest.to_json())

# convert the object into a dict
in_app_purchase_image_update_request_dict = in_app_purchase_image_update_request_instance.to_dict()
# create an instance of InAppPurchaseImageUpdateRequest from a dict
in_app_purchase_image_update_request_from_dict = InAppPurchaseImageUpdateRequest.from_dict(in_app_purchase_image_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


