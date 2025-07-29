# BetaFeedbackScreenshotSubmissionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_date** | **datetime** |  | [optional] 
**comment** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**device_model** | **str** |  | [optional] 
**os_version** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**architecture** | **str** |  | [optional] 
**connection_type** | [**DeviceConnectionType**](DeviceConnectionType.md) |  | [optional] 
**paired_apple_watch** | **str** |  | [optional] 
**app_uptime_in_milliseconds** | **int** |  | [optional] 
**disk_bytes_available** | **int** |  | [optional] 
**disk_bytes_total** | **int** |  | [optional] 
**battery_percentage** | **int** |  | [optional] 
**screen_width_in_points** | **int** |  | [optional] 
**screen_height_in_points** | **int** |  | [optional] 
**app_platform** | [**Platform**](Platform.md) |  | [optional] 
**device_platform** | [**Platform**](Platform.md) |  | [optional] 
**device_family** | [**DeviceFamily**](DeviceFamily.md) |  | [optional] 
**build_bundle_id** | **str** |  | [optional] 
**screenshots** | [**List[BetaFeedbackScreenshotImage]**](BetaFeedbackScreenshotImage.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_submission_attributes import BetaFeedbackScreenshotSubmissionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotSubmissionAttributes from a JSON string
beta_feedback_screenshot_submission_attributes_instance = BetaFeedbackScreenshotSubmissionAttributes.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotSubmissionAttributes.to_json())

# convert the object into a dict
beta_feedback_screenshot_submission_attributes_dict = beta_feedback_screenshot_submission_attributes_instance.to_dict()
# create an instance of BetaFeedbackScreenshotSubmissionAttributes from a dict
beta_feedback_screenshot_submission_attributes_from_dict = BetaFeedbackScreenshotSubmissionAttributes.from_dict(beta_feedback_screenshot_submission_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


