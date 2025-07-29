# BackgroundAssetVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetVersion**](BackgroundAssetVersion.md) |  | 
**included** | [**List[BackgroundAssetVersionsResponseIncludedInner]**](BackgroundAssetVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.background_asset_version_response import BackgroundAssetVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionResponse from a JSON string
background_asset_version_response_instance = BackgroundAssetVersionResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionResponse.to_json())

# convert the object into a dict
background_asset_version_response_dict = background_asset_version_response_instance.to_dict()
# create an instance of BackgroundAssetVersionResponse from a dict
background_asset_version_response_from_dict = BackgroundAssetVersionResponse.from_dict(background_asset_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


