# BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BackgroundAssetVersionRelationshipsAssetFileData]**](BackgroundAssetVersionRelationshipsAssetFileData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_version_background_asset_upload_files_linkages_response import BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse from a JSON string
background_asset_version_background_asset_upload_files_linkages_response_instance = BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.to_json())

# convert the object into a dict
background_asset_version_background_asset_upload_files_linkages_response_dict = background_asset_version_background_asset_upload_files_linkages_response_instance.to_dict()
# create an instance of BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse from a dict
background_asset_version_background_asset_upload_files_linkages_response_from_dict = BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.from_dict(background_asset_version_background_asset_upload_files_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


