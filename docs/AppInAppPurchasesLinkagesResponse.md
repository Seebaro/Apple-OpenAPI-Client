# AppInAppPurchasesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsInAppPurchasesDataInner]**](AppRelationshipsInAppPurchasesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_in_app_purchases_linkages_response import AppInAppPurchasesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppInAppPurchasesLinkagesResponse from a JSON string
app_in_app_purchases_linkages_response_instance = AppInAppPurchasesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppInAppPurchasesLinkagesResponse.to_json())

# convert the object into a dict
app_in_app_purchases_linkages_response_dict = app_in_app_purchases_linkages_response_instance.to_dict()
# create an instance of AppInAppPurchasesLinkagesResponse from a dict
app_in_app_purchases_linkages_response_from_dict = AppInAppPurchasesLinkagesResponse.from_dict(app_in_app_purchases_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


