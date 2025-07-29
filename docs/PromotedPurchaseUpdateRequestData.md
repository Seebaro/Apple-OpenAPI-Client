# PromotedPurchaseUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**PromotedPurchaseUpdateRequestDataAttributes**](PromotedPurchaseUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase_update_request_data import PromotedPurchaseUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseUpdateRequestData from a JSON string
promoted_purchase_update_request_data_instance = PromotedPurchaseUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseUpdateRequestData.to_json())

# convert the object into a dict
promoted_purchase_update_request_data_dict = promoted_purchase_update_request_data_instance.to_dict()
# create an instance of PromotedPurchaseUpdateRequestData from a dict
promoted_purchase_update_request_data_from_dict = PromotedPurchaseUpdateRequestData.from_dict(promoted_purchase_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


