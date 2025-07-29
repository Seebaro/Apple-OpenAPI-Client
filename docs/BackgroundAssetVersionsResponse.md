# BackgroundAssetVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BackgroundAssetVersion]**](BackgroundAssetVersion.md) |  | 
**included** | [**List[BackgroundAssetVersionsResponseIncludedInner]**](BackgroundAssetVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_versions_response import BackgroundAssetVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionsResponse from a JSON string
background_asset_versions_response_instance = BackgroundAssetVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionsResponse.to_json())

# convert the object into a dict
background_asset_versions_response_dict = background_asset_versions_response_instance.to_dict()
# create an instance of BackgroundAssetVersionsResponse from a dict
background_asset_versions_response_from_dict = BackgroundAssetVersionsResponse.from_dict(background_asset_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


