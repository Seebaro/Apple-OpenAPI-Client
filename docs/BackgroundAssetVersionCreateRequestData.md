# BackgroundAssetVersionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**BackgroundAssetVersionCreateRequestDataRelationships**](BackgroundAssetVersionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.background_asset_version_create_request_data import BackgroundAssetVersionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionCreateRequestData from a JSON string
background_asset_version_create_request_data_instance = BackgroundAssetVersionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionCreateRequestData.to_json())

# convert the object into a dict
background_asset_version_create_request_data_dict = background_asset_version_create_request_data_instance.to_dict()
# create an instance of BackgroundAssetVersionCreateRequestData from a dict
background_asset_version_create_request_data_from_dict = BackgroundAssetVersionCreateRequestData.from_dict(background_asset_version_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


