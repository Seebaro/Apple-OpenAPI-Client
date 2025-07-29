# BackgroundAssetUploadFileCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**BackgroundAssetUploadFileCreateRequestDataAttributes**](BackgroundAssetUploadFileCreateRequestDataAttributes.md) |  | 
**relationships** | [**BackgroundAssetUploadFileCreateRequestDataRelationships**](BackgroundAssetUploadFileCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.background_asset_upload_file_create_request_data import BackgroundAssetUploadFileCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetUploadFileCreateRequestData from a JSON string
background_asset_upload_file_create_request_data_instance = BackgroundAssetUploadFileCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetUploadFileCreateRequestData.to_json())

# convert the object into a dict
background_asset_upload_file_create_request_data_dict = background_asset_upload_file_create_request_data_instance.to_dict()
# create an instance of BackgroundAssetUploadFileCreateRequestData from a dict
background_asset_upload_file_create_request_data_from_dict = BackgroundAssetUploadFileCreateRequestData.from_dict(background_asset_upload_file_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


