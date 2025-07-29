# InAppPurchaseV2PricePointsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchasePriceRelationshipsInAppPurchasePricePointData]**](InAppPurchasePriceRelationshipsInAppPurchasePricePointData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_price_points_linkages_response import InAppPurchaseV2PricePointsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2PricePointsLinkagesResponse from a JSON string
in_app_purchase_v2_price_points_linkages_response_instance = InAppPurchaseV2PricePointsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2PricePointsLinkagesResponse.to_json())

# convert the object into a dict
in_app_purchase_v2_price_points_linkages_response_dict = in_app_purchase_v2_price_points_linkages_response_instance.to_dict()
# create an instance of InAppPurchaseV2PricePointsLinkagesResponse from a dict
in_app_purchase_v2_price_points_linkages_response_from_dict = InAppPurchaseV2PricePointsLinkagesResponse.from_dict(in_app_purchase_v2_price_points_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


