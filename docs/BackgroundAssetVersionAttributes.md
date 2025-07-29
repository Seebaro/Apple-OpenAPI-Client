# BackgroundAssetVersionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_date** | **datetime** |  | [optional] 
**platforms** | [**List[Platform]**](Platform.md) |  | [optional] 
**state** | [**BackgroundAssetVersionState**](BackgroundAssetVersionState.md) |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_version_attributes import BackgroundAssetVersionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionAttributes from a JSON string
background_asset_version_attributes_instance = BackgroundAssetVersionAttributes.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionAttributes.to_json())

# convert the object into a dict
background_asset_version_attributes_dict = background_asset_version_attributes_instance.to_dict()
# create an instance of BackgroundAssetVersionAttributes from a dict
background_asset_version_attributes_from_dict = BackgroundAssetVersionAttributes.from_dict(background_asset_version_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


