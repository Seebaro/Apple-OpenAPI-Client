# BetaAppReviewSubmissionWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaAppReviewSubmission**](BetaAppReviewSubmission.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_review_submission_without_includes_response import BetaAppReviewSubmissionWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppReviewSubmissionWithoutIncludesResponse from a JSON string
beta_app_review_submission_without_includes_response_instance = BetaAppReviewSubmissionWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppReviewSubmissionWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_app_review_submission_without_includes_response_dict = beta_app_review_submission_without_includes_response_instance.to_dict()
# create an instance of BetaAppReviewSubmissionWithoutIncludesResponse from a dict
beta_app_review_submission_without_includes_response_from_dict = BetaAppReviewSubmissionWithoutIncludesResponse.from_dict(beta_app_review_submission_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


