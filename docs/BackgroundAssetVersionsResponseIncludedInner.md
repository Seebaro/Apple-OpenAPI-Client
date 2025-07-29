# BackgroundAssetVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BackgroundAssetUploadFileAttributes**](BackgroundAssetUploadFileAttributes.md) |  | [optional] 
**relationships** | [**BackgroundAssetVersionInternalBetaReleaseRelationships**](BackgroundAssetVersionInternalBetaReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_versions_response_included_inner import BackgroundAssetVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionsResponseIncludedInner from a JSON string
background_asset_versions_response_included_inner_instance = BackgroundAssetVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionsResponseIncludedInner.to_json())

# convert the object into a dict
background_asset_versions_response_included_inner_dict = background_asset_versions_response_included_inner_instance.to_dict()
# create an instance of BackgroundAssetVersionsResponseIncludedInner from a dict
background_asset_versions_response_included_inner_from_dict = BackgroundAssetVersionsResponseIncludedInner.from_dict(background_asset_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


