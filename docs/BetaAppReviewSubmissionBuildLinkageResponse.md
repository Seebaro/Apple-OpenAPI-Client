# BetaAppReviewSubmissionBuildLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclarationRelationshipsBuildsDataInner**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_review_submission_build_linkage_response import BetaAppReviewSubmissionBuildLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppReviewSubmissionBuildLinkageResponse from a JSON string
beta_app_review_submission_build_linkage_response_instance = BetaAppReviewSubmissionBuildLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppReviewSubmissionBuildLinkageResponse.to_json())

# convert the object into a dict
beta_app_review_submission_build_linkage_response_dict = beta_app_review_submission_build_linkage_response_instance.to_dict()
# create an instance of BetaAppReviewSubmissionBuildLinkageResponse from a dict
beta_app_review_submission_build_linkage_response_from_dict = BetaAppReviewSubmissionBuildLinkageResponse.from_dict(beta_app_review_submission_build_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


