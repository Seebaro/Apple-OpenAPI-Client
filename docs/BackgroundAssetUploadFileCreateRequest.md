# BackgroundAssetUploadFileCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetUploadFileCreateRequestData**](BackgroundAssetUploadFileCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.background_asset_upload_file_create_request import BackgroundAssetUploadFileCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileCreateRequest from a JSON string
background_asset_upload_file_create_request_instance = BackgroundAssetUploadFileCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileCreateRequest.to_json())

# convert the object into a dict
background_asset_upload_file_create_request_dict = background_asset_upload_file_create_request_instance.to_dict()
# create an instance of BackgroundAssetUploadFileCreateRequest from a dict
background_asset_upload_file_create_request_from_dict = BackgroundAssetUploadFileCreateRequest.from_dict(background_asset_upload_file_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


