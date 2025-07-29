# BackgroundAssetsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BackgroundAsset]**](BackgroundAsset.md) |  | 
**included** | [**List[BackgroundAssetVersion]**](BackgroundAssetVersion.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_assets_response import BackgroundAssetsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetsResponse from a JSON string
background_assets_response_instance = BackgroundAssetsResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetsResponse.to_json())

# convert the object into a dict
background_assets_response_dict = background_assets_response_instance.to_dict()
# create an instance of BackgroundAssetsResponse from a dict
background_assets_response_from_dict = BackgroundAssetsResponse.from_dict(background_assets_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


