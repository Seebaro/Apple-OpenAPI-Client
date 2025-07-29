# BetaFeedbackScreenshotSubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaFeedbackScreenshotSubmission**](BetaFeedbackScreenshotSubmission.md) |  | 
**included** | [**List[BetaFeedbackCrashSubmissionsResponseIncludedInner]**](BetaFeedbackCrashSubmissionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_submission_response import BetaFeedbackScreenshotSubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotSubmissionResponse from a JSON string
beta_feedback_screenshot_submission_response_instance = BetaFeedbackScreenshotSubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotSubmissionResponse.to_json())

# convert the object into a dict
beta_feedback_screenshot_submission_response_dict = beta_feedback_screenshot_submission_response_instance.to_dict()
# create an instance of BetaFeedbackScreenshotSubmissionResponse from a dict
beta_feedback_screenshot_submission_response_from_dict = BetaFeedbackScreenshotSubmissionResponse.from_dict(beta_feedback_screenshot_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


