# BackgroundAssetUploadFilesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BackgroundAssetUploadFile]**](BackgroundAssetUploadFile.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_upload_files_response import BackgroundAssetUploadFilesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFilesResponse from a JSON string
background_asset_upload_files_response_instance = BackgroundAssetUploadFilesResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFilesResponse.to_json())

# convert the object into a dict
background_asset_upload_files_response_dict = background_asset_upload_files_response_instance.to_dict()
# create an instance of BackgroundAssetUploadFilesResponse from a dict
background_asset_upload_files_response_from_dict = BackgroundAssetUploadFilesResponse.from_dict(background_asset_upload_files_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


