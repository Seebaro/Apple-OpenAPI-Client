# BetaFeedbackScreenshotSubmissionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaFeedbackScreenshotSubmission]**](BetaFeedbackScreenshotSubmission.md) |  | 
**included** | [**List[BetaFeedbackCrashSubmissionsResponseIncludedInner]**](BetaFeedbackCrashSubmissionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_submissions_response import BetaFeedbackScreenshotSubmissionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotSubmissionsResponse from a JSON string
beta_feedback_screenshot_submissions_response_instance = BetaFeedbackScreenshotSubmissionsResponse.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotSubmissionsResponse.to_json())

# convert the object into a dict
beta_feedback_screenshot_submissions_response_dict = beta_feedback_screenshot_submissions_response_instance.to_dict()
# create an instance of BetaFeedbackScreenshotSubmissionsResponse from a dict
beta_feedback_screenshot_submissions_response_from_dict = BetaFeedbackScreenshotSubmissionsResponse.from_dict(beta_feedback_screenshot_submissions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


