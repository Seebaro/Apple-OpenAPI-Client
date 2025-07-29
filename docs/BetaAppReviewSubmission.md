# BetaAppReviewSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaAppReviewSubmissionAttributes**](BetaAppReviewSubmissionAttributes.md) |  | [optional] 
**relationships** | [**BetaAppReviewSubmissionRelationships**](BetaAppReviewSubmissionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_review_submission import BetaAppReviewSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppReviewSubmission from a JSON string
beta_app_review_submission_instance = BetaAppReviewSubmission.from_json(json)
# print the JSON string representation of the object
print(BetaAppReviewSubmission.to_json())

# convert the object into a dict
beta_app_review_submission_dict = beta_app_review_submission_instance.to_dict()
# create an instance of BetaAppReviewSubmission from a dict
beta_app_review_submission_from_dict = BetaAppReviewSubmission.from_dict(beta_app_review_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


