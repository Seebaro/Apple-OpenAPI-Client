# InAppPurchasePricePointsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchasePricePoint]**](InAppPurchasePricePoint.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_points_response import InAppPurchasePricePointsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePricePointsResponse from a JSON string
in_app_purchase_price_points_response_instance = InAppPurchasePricePointsResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePricePointsResponse.to_json())

# convert the object into a dict
in_app_purchase_price_points_response_dict = in_app_purchase_price_points_response_instance.to_dict()
# create an instance of InAppPurchasePricePointsResponse from a dict
in_app_purchase_price_points_response_from_dict = InAppPurchasePricePointsResponse.from_dict(in_app_purchase_price_points_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


