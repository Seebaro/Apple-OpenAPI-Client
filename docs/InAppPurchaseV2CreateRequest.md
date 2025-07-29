# InAppPurchaseV2CreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseV2CreateRequestData**](InAppPurchaseV2CreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_v2_create_request import InAppPurchaseV2CreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2CreateRequest from a JSON string
in_app_purchase_v2_create_request_instance = InAppPurchaseV2CreateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2CreateRequest.to_json())

# convert the object into a dict
in_app_purchase_v2_create_request_dict = in_app_purchase_v2_create_request_instance.to_dict()
# create an instance of InAppPurchaseV2CreateRequest from a dict
in_app_purchase_v2_create_request_from_dict = InAppPurchaseV2CreateRequest.from_dict(in_app_purchase_v2_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


