# PromotedPurchaseCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**visible_for_all_users** | **bool** |  | 
**enabled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase_create_request_data_attributes import PromotedPurchaseCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseCreateRequestDataAttributes from a JSON string
promoted_purchase_create_request_data_attributes_instance = PromotedPurchaseCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseCreateRequestDataAttributes.to_json())

# convert the object into a dict
promoted_purchase_create_request_data_attributes_dict = promoted_purchase_create_request_data_attributes_instance.to_dict()
# create an instance of PromotedPurchaseCreateRequestDataAttributes from a dict
promoted_purchase_create_request_data_attributes_from_dict = PromotedPurchaseCreateRequestDataAttributes.from_dict(promoted_purchase_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


