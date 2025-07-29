# AppBackgroundAssetsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BackgroundAssetVersionCreateRequestDataRelationshipsBackgroundAssetData]**](BackgroundAssetVersionCreateRequestDataRelationshipsBackgroundAssetData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_background_assets_linkages_response import AppBackgroundAssetsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppBackgroundAssetsLinkagesResponse from a JSON string
app_background_assets_linkages_response_instance = AppBackgroundAssetsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppBackgroundAssetsLinkagesResponse.to_json())

# convert the object into a dict
app_background_assets_linkages_response_dict = app_background_assets_linkages_response_instance.to_dict()
# create an instance of AppBackgroundAssetsLinkagesResponse from a dict
app_background_assets_linkages_response_from_dict = AppBackgroundAssetsLinkagesResponse.from_dict(app_background_assets_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


