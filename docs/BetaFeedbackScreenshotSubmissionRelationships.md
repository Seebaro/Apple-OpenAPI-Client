# BetaFeedbackScreenshotSubmissionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**build** | [**AppStoreVersionCreateRequestDataRelationshipsBuild**](AppStoreVersionCreateRequestDataRelationshipsBuild.md) |  | [optional] 
**tester** | [**BetaFeedbackCrashSubmissionRelationshipsTester**](BetaFeedbackCrashSubmissionRelationshipsTester.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_screenshot_submission_relationships import BetaFeedbackScreenshotSubmissionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackScreenshotSubmissionRelationships from a JSON string
beta_feedback_screenshot_submission_relationships_instance = BetaFeedbackScreenshotSubmissionRelationships.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackScreenshotSubmissionRelationships.to_json())

# convert the object into a dict
beta_feedback_screenshot_submission_relationships_dict = beta_feedback_screenshot_submission_relationships_instance.to_dict()
# create an instance of BetaFeedbackScreenshotSubmissionRelationships from a dict
beta_feedback_screenshot_submission_relationships_from_dict = BetaFeedbackScreenshotSubmissionRelationships.from_dict(beta_feedback_screenshot_submission_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


