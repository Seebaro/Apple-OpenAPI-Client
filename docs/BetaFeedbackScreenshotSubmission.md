# BetaFeedbackScreenshotSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaFeedbackScreenshotSubmissionAttributes**](BetaFeedbackScreenshotSubmissionAttributes.md) |  | [optional] 
**relationships** | [**BetaFeedbackScreenshotSubmissionRelationships**](BetaFeedbackScreenshotSubmissionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_submission import BetaFeedbackScreenshotSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotSubmission from a JSON string
beta_feedback_screenshot_submission_instance = BetaFeedbackScreenshotSubmission.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotSubmission.to_json())

# convert the object into a dict
beta_feedback_screenshot_submission_dict = beta_feedback_screenshot_submission_instance.to_dict()
# create an instance of BetaFeedbackScreenshotSubmission from a dict
beta_feedback_screenshot_submission_from_dict = BetaFeedbackScreenshotSubmission.from_dict(beta_feedback_screenshot_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


