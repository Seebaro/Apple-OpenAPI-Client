# AppPromotedPurchasesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsPromotedPurchasesDataInner]**](AppRelationshipsPromotedPurchasesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_promoted_purchases_linkages_response import AppPromotedPurchasesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPromotedPurchasesLinkagesResponse from a JSON string
app_promoted_purchases_linkages_response_instance = AppPromotedPurchasesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPromotedPurchasesLinkagesResponse.to_json())

# convert the object into a dict
app_promoted_purchases_linkages_response_dict = app_promoted_purchases_linkages_response_instance.to_dict()
# create an instance of AppPromotedPurchasesLinkagesResponse from a dict
app_promoted_purchases_linkages_response_from_dict = AppPromotedPurchasesLinkagesResponse.from_dict(app_promoted_purchases_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


