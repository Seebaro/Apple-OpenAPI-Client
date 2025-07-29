# AppAppPricePointsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPriceV2RelationshipsAppPricePointData]**](AppPriceV2RelationshipsAppPricePointData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_price_points_linkages_response import AppAppPricePointsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppPricePointsLinkagesResponse from a JSON string
app_app_price_points_linkages_response_instance = AppAppPricePointsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppPricePointsLinkagesResponse.to_json())

# convert the object into a dict
app_app_price_points_linkages_response_dict = app_app_price_points_linkages_response_instance.to_dict()
# create an instance of AppAppPricePointsLinkagesResponse from a dict
app_app_price_points_linkages_response_from_dict = AppAppPricePointsLinkagesResponse.from_dict(app_app_price_points_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


