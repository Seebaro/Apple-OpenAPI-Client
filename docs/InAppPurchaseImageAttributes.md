# InAppPurchaseImageAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**source_file_checksum** | **str** |  | [optional] 
**asset_token** | **str** |  | [optional] 
**image_asset** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_image_attributes import InAppPurchaseImageAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseImageAttributes from a JSON string
in_app_purchase_image_attributes_instance = InAppPurchaseImageAttributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseImageAttributes.to_json())

# convert the object into a dict
in_app_purchase_image_attributes_dict = in_app_purchase_image_attributes_instance.to_dict()
# create an instance of InAppPurchaseImageAttributes from a dict
in_app_purchase_image_attributes_from_dict = InAppPurchaseImageAttributes.from_dict(in_app_purchase_image_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


