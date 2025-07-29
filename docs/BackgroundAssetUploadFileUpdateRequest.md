# BackgroundAssetUploadFileUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetUploadFileUpdateRequestData**](BackgroundAssetUploadFileUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.background_asset_upload_file_update_request import BackgroundAssetUploadFileUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileUpdateRequest from a JSON string
background_asset_upload_file_update_request_instance = BackgroundAssetUploadFileUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileUpdateRequest.to_json())

# convert the object into a dict
background_asset_upload_file_update_request_dict = background_asset_upload_file_update_request_instance.to_dict()
# create an instance of BackgroundAssetUploadFileUpdateRequest from a dict
background_asset_upload_file_update_request_from_dict = BackgroundAssetUploadFileUpdateRequest.from_dict(background_asset_upload_file_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


