# BackgroundAssetVersionInternalBetaReleaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetVersionInternalBetaRelease**](BackgroundAssetVersionInternalBetaRelease.md) |  | 
**included** | [**List[BackgroundAssetVersion]**](BackgroundAssetVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.background_asset_version_internal_beta_release_response import BackgroundAssetVersionInternalBetaReleaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionInternalBetaReleaseResponse from a JSON string
background_asset_version_internal_beta_release_response_instance = BackgroundAssetVersionInternalBetaReleaseResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionInternalBetaReleaseResponse.to_json())

# convert the object into a dict
background_asset_version_internal_beta_release_response_dict = background_asset_version_internal_beta_release_response_instance.to_dict()
# create an instance of BackgroundAssetVersionInternalBetaReleaseResponse from a dict
background_asset_version_internal_beta_release_response_from_dict = BackgroundAssetVersionInternalBetaReleaseResponse.from_dict(background_asset_version_internal_beta_release_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


