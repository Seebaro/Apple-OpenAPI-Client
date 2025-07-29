# BetaFeedbackCrashSubmissionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaFeedbackCrashSubmission]**](BetaFeedbackCrashSubmission.md) |  | 
**included** | [**List[BetaFeedbackCrashSubmissionsResponseIncludedInner]**](BetaFeedbackCrashSubmissionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_crash_submissions_response import BetaFeedbackCrashSubmissionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackCrashSubmissionsResponse from a JSON string
beta_feedback_crash_submissions_response_instance = BetaFeedbackCrashSubmissionsResponse.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackCrashSubmissionsResponse.to_json())

# convert the object into a dict
beta_feedback_crash_submissions_response_dict = beta_feedback_crash_submissions_response_instance.to_dict()
# create an instance of BetaFeedbackCrashSubmissionsResponse from a dict
beta_feedback_crash_submissions_response_from_dict = BetaFeedbackCrashSubmissionsResponse.from_dict(beta_feedback_crash_submissions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


