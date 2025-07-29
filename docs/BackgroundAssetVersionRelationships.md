# BackgroundAssetVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**internal_beta_release** | [**BackgroundAssetVersionRelationshipsInternalBetaRelease**](BackgroundAssetVersionRelationshipsInternalBetaRelease.md) |  | [optional] 
**asset_file** | [**BackgroundAssetVersionRelationshipsAssetFile**](BackgroundAssetVersionRelationshipsAssetFile.md) |  | [optional] 
**manifest_file** | [**BackgroundAssetVersionRelationshipsAssetFile**](BackgroundAssetVersionRelationshipsAssetFile.md) |  | [optional] 
**background_asset_upload_files** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_version_relationships import BackgroundAssetVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionRelationships from a JSON string
background_asset_version_relationships_instance = BackgroundAssetVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionRelationships.to_json())

# convert the object into a dict
background_asset_version_relationships_dict = background_asset_version_relationships_instance.to_dict()
# create an instance of BackgroundAssetVersionRelationships from a dict
background_asset_version_relationships_from_dict = BackgroundAssetVersionRelationships.from_dict(background_asset_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


