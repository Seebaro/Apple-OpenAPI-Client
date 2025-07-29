# AppEventScreenshotCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | 
**file_name** | **str** |  | 
**app_event_asset_type** | [**AppEventAssetType**](AppEventAssetType.md) |  | 

## Example

```python
from openapi_client.models.app_event_screenshot_create_request_data_attributes import AppEventScreenshotCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotCreateRequestDataAttributes from a JSON string
app_event_screenshot_create_request_data_attributes_instance = AppEventScreenshotCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotCreateRequestDataAttributes.to_json())

# convert the object into a dict
app_event_screenshot_create_request_data_attributes_dict = app_event_screenshot_create_request_data_attributes_instance.to_dict()
# create an instance of AppEventScreenshotCreateRequestDataAttributes from a dict
app_event_screenshot_create_request_data_attributes_from_dict = AppEventScreenshotCreateRequestDataAttributes.from_dict(app_event_screenshot_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


