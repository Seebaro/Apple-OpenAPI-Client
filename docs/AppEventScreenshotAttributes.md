# AppEventScreenshotAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**image_asset** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**asset_token** | **str** |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 
**app_event_asset_type** | [**AppEventAssetType**](AppEventAssetType.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_screenshot_attributes import AppEventScreenshotAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotAttributes from a JSON string
app_event_screenshot_attributes_instance = AppEventScreenshotAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotAttributes.to_json())

# convert the object into a dict
app_event_screenshot_attributes_dict = app_event_screenshot_attributes_instance.to_dict()
# create an instance of AppEventScreenshotAttributes from a dict
app_event_screenshot_attributes_from_dict = AppEventScreenshotAttributes.from_dict(app_event_screenshot_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


