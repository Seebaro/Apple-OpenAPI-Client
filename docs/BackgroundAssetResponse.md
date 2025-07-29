# BackgroundAssetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAsset**](BackgroundAsset.md) |  | 
**included** | [**List[BackgroundAssetVersion]**](BackgroundAssetVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.background_asset_response import BackgroundAssetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetResponse from a JSON string
background_asset_response_instance = BackgroundAssetResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetResponse.to_json())

# convert the object into a dict
background_asset_response_dict = background_asset_response_instance.to_dict()
# create an instance of BackgroundAssetResponse from a dict
background_asset_response_from_dict = BackgroundAssetResponse.from_dict(background_asset_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


