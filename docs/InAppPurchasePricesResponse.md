# InAppPurchasePricesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchasePrice]**](InAppPurchasePrice.md) |  | 
**included** | [**List[InAppPurchasePricesResponseIncludedInner]**](InAppPurchasePricesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_prices_response import InAppPurchasePricesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePricesResponse from a JSON string
in_app_purchase_prices_response_instance = InAppPurchasePricesResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePricesResponse.to_json())

# convert the object into a dict
in_app_purchase_prices_response_dict = in_app_purchase_prices_response_instance.to_dict()
# create an instance of InAppPurchasePricesResponse from a dict
in_app_purchase_prices_response_from_dict = InAppPurchasePricesResponse.from_dict(in_app_purchase_prices_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


