# BackgroundAssetRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**versions** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**internal_beta_version** | [**BackgroundAssetVersionInternalBetaReleaseRelationshipsBackgroundAssetVersion**](BackgroundAssetVersionInternalBetaReleaseRelationshipsBackgroundAssetVersion.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_relationships import BackgroundAssetRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetRelationships from a JSON string
background_asset_relationships_instance = BackgroundAssetRelationships.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetRelationships.to_json())

# convert the object into a dict
background_asset_relationships_dict = background_asset_relationships_instance.to_dict()
# create an instance of BackgroundAssetRelationships from a dict
background_asset_relationships_from_dict = BackgroundAssetRelationships.from_dict(background_asset_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


