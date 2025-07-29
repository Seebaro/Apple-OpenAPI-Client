# AppPromotedPurchasesLinkagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsPromotedPurchasesDataInner]**](AppRelationshipsPromotedPurchasesDataInner.md) |  | 

## Example

```python
from openapi_client.models.app_promoted_purchases_linkages_request import AppPromotedPurchasesLinkagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppPromotedPurchasesLinkagesRequest from a JSON string
app_promoted_purchases_linkages_request_instance = AppPromotedPurchasesLinkagesRequest.from_json(json)
# print the JSON string representation of the object
print(AppPromotedPurchasesLinkagesRequest.to_json())

# convert the object into a dict
app_promoted_purchases_linkages_request_dict = app_promoted_purchases_linkages_request_instance.to_dict()
# create an instance of AppPromotedPurchasesLinkagesRequest from a dict
app_promoted_purchases_linkages_request_from_dict = AppPromotedPurchasesLinkagesRequest.from_dict(app_promoted_purchases_linkages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


