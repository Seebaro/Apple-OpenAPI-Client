# BackgroundAssetUploadFileAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 
**asset_token** | **str** |  | [optional] 
**asset_type** | **str** |  | [optional] 
**file_name** | **str** |  | [optional] 
**file_size** | **int** |  | [optional] 
**source_file_checksum** | **str** |  | [optional] 
**upload_operations** | [**List[DeliveryFileUploadOperation]**](DeliveryFileUploadOperation.md) |  | [optional] 

## Example

```python
from openapi_client.models.background_asset_upload_file_attributes import BackgroundAssetUploadFileAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileAttributes from a JSON string
background_asset_upload_file_attributes_instance = BackgroundAssetUploadFileAttributes.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileAttributes.to_json())

# convert the object into a dict
background_asset_upload_file_attributes_dict = background_asset_upload_file_attributes_instance.to_dict()
# create an instance of BackgroundAssetUploadFileAttributes from a dict
background_asset_upload_file_attributes_from_dict = BackgroundAssetUploadFileAttributes.from_dict(background_asset_upload_file_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


