# PromotedPurchasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PromotedPurchase]**](PromotedPurchase.md) |  | 
**included** | [**List[PromotedPurchasesResponseIncludedInner]**](PromotedPurchasesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchases_response import PromotedPurchasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchasesResponse from a JSON string
promoted_purchases_response_instance = PromotedPurchasesResponse.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchasesResponse.to_json())

# convert the object into a dict
promoted_purchases_response_dict = promoted_purchases_response_instance.to_dict()
# create an instance of PromotedPurchasesResponse from a dict
promoted_purchases_response_from_dict = PromotedPurchasesResponse.from_dict(promoted_purchases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


