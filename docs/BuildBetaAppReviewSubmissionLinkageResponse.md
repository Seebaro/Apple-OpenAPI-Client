# BuildBetaAppReviewSubmissionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BuildRelationshipsBetaAppReviewSubmissionData**](BuildRelationshipsBetaAppReviewSubmissionData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_beta_app_review_submission_linkage_response import BuildBetaAppReviewSubmissionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBetaAppReviewSubmissionLinkageResponse from a JSON string
build_beta_app_review_submission_linkage_response_instance = BuildBetaAppReviewSubmissionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BuildBetaAppReviewSubmissionLinkageResponse.to_json())

# convert the object into a dict
build_beta_app_review_submission_linkage_response_dict = build_beta_app_review_submission_linkage_response_instance.to_dict()
# create an instance of BuildBetaAppReviewSubmissionLinkageResponse from a dict
build_beta_app_review_submission_linkage_response_from_dict = BuildBetaAppReviewSubmissionLinkageResponse.from_dict(build_beta_app_review_submission_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


