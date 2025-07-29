# BackgroundAssetUploadFile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BackgroundAssetUploadFileAttributes**](BackgroundAssetUploadFileAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_upload_file import BackgroundAssetUploadFile

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFile from a JSON string
background_asset_upload_file_instance = BackgroundAssetUploadFile.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFile.to_json())

# convert the object into a dict
background_asset_upload_file_dict = background_asset_upload_file_instance.to_dict()
# create an instance of BackgroundAssetUploadFile from a dict
background_asset_upload_file_from_dict = BackgroundAssetUploadFile.from_dict(background_asset_upload_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


