# BetaFeedbackCrashSubmissionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**crash_log** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**build** | [**AppStoreVersionCreateRequestDataRelationshipsBuild**](AppStoreVersionCreateRequestDataRelationshipsBuild.md) |  | [optional] 
**tester** | [**BetaFeedbackCrashSubmissionRelationshipsTester**](BetaFeedbackCrashSubmissionRelationshipsTester.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_crash_submission_relationships import BetaFeedbackCrashSubmissionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackCrashSubmissionRelationships from a JSON string
beta_feedback_crash_submission_relationships_instance = BetaFeedbackCrashSubmissionRelationships.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackCrashSubmissionRelationships.to_json())

# convert the object into a dict
beta_feedback_crash_submission_relationships_dict = beta_feedback_crash_submission_relationships_instance.to_dict()
# create an instance of BetaFeedbackCrashSubmissionRelationships from a dict
beta_feedback_crash_submission_relationships_from_dict = BetaFeedbackCrashSubmissionRelationships.from_dict(beta_feedback_crash_submission_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


