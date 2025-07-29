# BackgroundAssetUploadFileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetUploadFile**](BackgroundAssetUploadFile.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.background_asset_upload_file_response import BackgroundAssetUploadFileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileResponse from a JSON string
background_asset_upload_file_response_instance = BackgroundAssetUploadFileResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileResponse.to_json())

# convert the object into a dict
background_asset_upload_file_response_dict = background_asset_upload_file_response_instance.to_dict()
# create an instance of BackgroundAssetUploadFileResponse from a dict
background_asset_upload_file_response_from_dict = BackgroundAssetUploadFileResponse.from_dict(background_asset_upload_file_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


