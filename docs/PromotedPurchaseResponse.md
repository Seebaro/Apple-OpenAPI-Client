# PromotedPurchaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PromotedPurchase**](PromotedPurchase.md) |  | 
**included** | [**List[PromotedPurchasesResponseIncludedInner]**](PromotedPurchasesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.promoted_purchase_response import PromotedPurchaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseResponse from a JSON string
promoted_purchase_response_instance = PromotedPurchaseResponse.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseResponse.to_json())

# convert the object into a dict
promoted_purchase_response_dict = promoted_purchase_response_instance.to_dict()
# create an instance of PromotedPurchaseResponse from a dict
promoted_purchase_response_from_dict = PromotedPurchaseResponse.from_dict(promoted_purchase_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


