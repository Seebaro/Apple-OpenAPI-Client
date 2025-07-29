# BetaFeedbackCrashSubmissionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaTesterAttributes**](BetaTesterAttributes.md) |  | [optional] 
**relationships** | [**BetaTesterRelationships**](BetaTesterRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_feedback_crash_submissions_response_included_inner import BetaFeedbackCrashSubmissionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of BetaFeedbackCrashSubmissionsResponseIncludedInner from a JSON string
beta_feedback_crash_submissions_response_included_inner_instance = BetaFeedbackCrashSubmissionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(BetaFeedbackCrashSubmissionsResponseIncludedInner.to_json())

# convert the object into a dict
beta_feedback_crash_submissions_response_included_inner_dict = beta_feedback_crash_submissions_response_included_inner_instance.to_dict()
# create an instance of BetaFeedbackCrashSubmissionsResponseIncludedInner from a dict
beta_feedback_crash_submissions_response_included_inner_from_dict = BetaFeedbackCrashSubmissionsResponseIncludedInner.from_dict(beta_feedback_crash_submissions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


