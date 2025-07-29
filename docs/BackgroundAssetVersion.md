# BackgroundAssetVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BackgroundAssetVersionAttributes**](BackgroundAssetVersionAttributes.md) |  | [optional] 
**relationships** | [**BackgroundAssetVersionRelationships**](BackgroundAssetVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_version import BackgroundAssetVersion

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersion from a JSON string
background_asset_version_instance = BackgroundAssetVersion.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersion.to_json())

# convert the object into a dict
background_asset_version_dict = background_asset_version_instance.to_dict()
# create an instance of BackgroundAssetVersion from a dict
background_asset_version_from_dict = BackgroundAssetVersion.from_dict(background_asset_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


