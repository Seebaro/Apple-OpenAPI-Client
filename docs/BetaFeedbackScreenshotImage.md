# BetaFeedbackScreenshotImage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**width** | **int** |  | [optional] 
**height** | **int** |  | [optional] 
**expiration_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_image import BetaFeedbackScreenshotImage

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotImage from a JSON string
beta_feedback_screenshot_image_instance = BetaFeedbackScreenshotImage.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotImage.to_json())

# convert the object into a dict
beta_feedback_screenshot_image_dict = beta_feedback_screenshot_image_instance.to_dict()
# create an instance of BetaFeedbackScreenshotImage from a dict
beta_feedback_screenshot_image_from_dict = BetaFeedbackScreenshotImage.from_dict(beta_feedback_screenshot_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


