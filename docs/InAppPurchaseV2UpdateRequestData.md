# InAppPurchaseV2UpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseV2UpdateRequestDataAttributes**](InAppPurchaseV2UpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_update_request_data import InAppPurchaseV2UpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2UpdateRequestData from a JSON string
in_app_purchase_v2_update_request_data_instance = InAppPurchaseV2UpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2UpdateRequestData.to_json())

# convert the object into a dict
in_app_purchase_v2_update_request_data_dict = in_app_purchase_v2_update_request_data_instance.to_dict()
# create an instance of InAppPurchaseV2UpdateRequestData from a dict
in_app_purchase_v2_update_request_data_from_dict = InAppPurchaseV2UpdateRequestData.from_dict(in_app_purchase_v2_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


