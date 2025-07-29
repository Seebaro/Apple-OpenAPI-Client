# BackgroundAssetVersionInternalBetaRelease


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BackgroundAssetVersionInternalBetaReleaseAttributes**](BackgroundAssetVersionInternalBetaReleaseAttributes.md) |  | [optional] 
**relationships** | [**BackgroundAssetVersionInternalBetaReleaseRelationships**](BackgroundAssetVersionInternalBetaReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_version_internal_beta_release import BackgroundAssetVersionInternalBetaRelease

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionInternalBetaRelease from a JSON string
background_asset_version_internal_beta_release_instance = BackgroundAssetVersionInternalBetaRelease.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionInternalBetaRelease.to_json())

# convert the object into a dict
background_asset_version_internal_beta_release_dict = background_asset_version_internal_beta_release_instance.to_dict()
# create an instance of BackgroundAssetVersionInternalBetaRelease from a dict
background_asset_version_internal_beta_release_from_dict = BackgroundAssetVersionInternalBetaRelease.from_dict(background_asset_version_internal_beta_release_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


