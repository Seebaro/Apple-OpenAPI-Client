# BackgroundAssetUploadFileCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset_type** | **str** |  | 
**file_name** | **str** |  | 
**file_size** | **int** |  | 

## Example

```python
from openapi_client.models.background_asset_upload_file_create_request_data_attributes import BackgroundAssetUploadFileCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileCreateRequestDataAttributes from a JSON string
background_asset_upload_file_create_request_data_attributes_instance = BackgroundAssetUploadFileCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileCreateRequestDataAttributes.to_json())

# convert the object into a dict
background_asset_upload_file_create_request_data_attributes_dict = background_asset_upload_file_create_request_data_attributes_instance.to_dict()
# create an instance of BackgroundAssetUploadFileCreateRequestDataAttributes from a dict
background_asset_upload_file_create_request_data_attributes_from_dict = BackgroundAssetUploadFileCreateRequestDataAttributes.from_dict(background_asset_upload_file_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


