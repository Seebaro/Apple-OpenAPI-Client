# PromotedPurchaseCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**PromotedPurchaseCreateRequestDataAttributes**](PromotedPurchaseCreateRequestDataAttributes.md) |  | 
**relationships** | [**PromotedPurchaseCreateRequestDataRelationships**](PromotedPurchaseCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.promoted_purchase_create_request_data import PromotedPurchaseCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseCreateRequestData from a JSON string
promoted_purchase_create_request_data_instance = PromotedPurchaseCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseCreateRequestData.to_json())

# convert the object into a dict
promoted_purchase_create_request_data_dict = promoted_purchase_create_request_data_instance.to_dict()
# create an instance of PromotedPurchaseCreateRequestData from a dict
promoted_purchase_create_request_data_from_dict = PromotedPurchaseCreateRequestData.from_dict(promoted_purchase_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


