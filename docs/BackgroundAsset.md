# BackgroundAsset


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BackgroundAssetAttributes**](BackgroundAssetAttributes.md) |  | [optional] 
**relationships** | [**BackgroundAssetRelationships**](BackgroundAssetRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset import BackgroundAsset

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAsset from a JSON string
background_asset_instance = BackgroundAsset.from_json(json)
# print the JSON string representation of the object
print(BackgroundAsset.to_json())

# convert the object into a dict
background_asset_dict = background_asset_instance.to_dict()
# create an instance of BackgroundAsset from a dict
background_asset_from_dict = BackgroundAsset.from_dict(background_asset_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


