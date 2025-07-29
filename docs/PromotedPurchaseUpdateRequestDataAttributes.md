# PromotedPurchaseUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**visible_for_all_users** | **bool** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase_update_request_data_attributes import PromotedPurchaseUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseUpdateRequestDataAttributes from a JSON string
promoted_purchase_update_request_data_attributes_instance = PromotedPurchaseUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseUpdateRequestDataAttributes.to_json())

# convert the object into a dict
promoted_purchase_update_request_data_attributes_dict = promoted_purchase_update_request_data_attributes_instance.to_dict()
# create an instance of PromotedPurchaseUpdateRequestDataAttributes from a dict
promoted_purchase_update_request_data_attributes_from_dict = PromotedPurchaseUpdateRequestDataAttributes.from_dict(promoted_purchase_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


