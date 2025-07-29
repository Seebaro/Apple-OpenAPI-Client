# AppMarketplaceSearchDetailLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppMarketplaceSearchDetailLinkageResponseData**](AppMarketplaceSearchDetailLinkageResponseData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_marketplace_search_detail_linkage_response import AppMarketplaceSearchDetailLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppMarketplaceSearchDetailLinkageResponse from a JSON string
app_marketplace_search_detail_linkage_response_instance = AppMarketplaceSearchDetailLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppMarketplaceSearchDetailLinkageResponse.to_json())

# convert the object into a dict
app_marketplace_search_detail_linkage_response_dict = app_marketplace_search_detail_linkage_response_instance.to_dict()
# create an instance of AppMarketplaceSearchDetailLinkageResponse from a dict
app_marketplace_search_detail_linkage_response_from_dict = AppMarketplaceSearchDetailLinkageResponse.from_dict(app_marketplace_search_detail_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


