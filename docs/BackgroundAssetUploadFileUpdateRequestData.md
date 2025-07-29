# BackgroundAssetUploadFileUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_upload_file_update_request_data import BackgroundAssetUploadFileUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileUpdateRequestData from a JSON string
background_asset_upload_file_update_request_data_instance = BackgroundAssetUploadFileUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileUpdateRequestData.to_json())

# convert the object into a dict
background_asset_upload_file_update_request_data_dict = background_asset_upload_file_update_request_data_instance.to_dict()
# create an instance of BackgroundAssetUploadFileUpdateRequestData from a dict
background_asset_upload_file_update_request_data_from_dict = BackgroundAssetUploadFileUpdateRequestData.from_dict(background_asset_upload_file_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


