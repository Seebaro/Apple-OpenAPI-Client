# InAppPurchaseV2UpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseV2UpdateRequestData**](InAppPurchaseV2UpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_v2_update_request import InAppPurchaseV2UpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2UpdateRequest from a JSON string
in_app_purchase_v2_update_request_instance = InAppPurchaseV2UpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2UpdateRequest.to_json())

# convert the object into a dict
in_app_purchase_v2_update_request_dict = in_app_purchase_v2_update_request_instance.to_dict()
# create an instance of InAppPurchaseV2UpdateRequest from a dict
in_app_purchase_v2_update_request_from_dict = InAppPurchaseV2UpdateRequest.from_dict(in_app_purchase_v2_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


