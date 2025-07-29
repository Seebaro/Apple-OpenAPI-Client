# InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchaseV2RelationshipsInAppPurchaseLocalizationsDataInner]**](InAppPurchaseV2RelationshipsInAppPurchaseLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_in_app_purchase_localizations_linkages_response import InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse from a JSON string
in_app_purchase_v2_in_app_purchase_localizations_linkages_response_instance = InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
in_app_purchase_v2_in_app_purchase_localizations_linkages_response_dict = in_app_purchase_v2_in_app_purchase_localizations_linkages_response_instance.to_dict()
# create an instance of InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse from a dict
in_app_purchase_v2_in_app_purchase_localizations_linkages_response_from_dict = InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse.from_dict(in_app_purchase_v2_in_app_purchase_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


