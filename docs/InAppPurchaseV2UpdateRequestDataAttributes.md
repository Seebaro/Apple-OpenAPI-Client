# InAppPurchaseV2UpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**review_note** | **str** |  | [optional] 
**family_sharable** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_update_request_data_attributes import InAppPurchaseV2UpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2UpdateRequestDataAttributes from a JSON string
in_app_purchase_v2_update_request_data_attributes_instance = InAppPurchaseV2UpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2UpdateRequestDataAttributes.to_json())

# convert the object into a dict
in_app_purchase_v2_update_request_data_attributes_dict = in_app_purchase_v2_update_request_data_attributes_instance.to_dict()
# create an instance of InAppPurchaseV2UpdateRequestDataAttributes from a dict
in_app_purchase_v2_update_request_data_attributes_from_dict = InAppPurchaseV2UpdateRequestDataAttributes.from_dict(in_app_purchase_v2_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


