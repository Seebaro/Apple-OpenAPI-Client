# BackgroundAssetAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset_pack_identifier** | **str** |  | [optional] 
**created_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_attributes import BackgroundAssetAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetAttributes from a JSON string
background_asset_attributes_instance = BackgroundAssetAttributes.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetAttributes.to_json())

# convert the object into a dict
background_asset_attributes_dict = background_asset_attributes_instance.to_dict()
# create an instance of BackgroundAssetAttributes from a dict
background_asset_attributes_from_dict = BackgroundAssetAttributes.from_dict(background_asset_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


