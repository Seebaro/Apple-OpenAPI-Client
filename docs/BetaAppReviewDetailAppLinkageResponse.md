# BetaAppReviewDetailAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_review_detail_app_linkage_response import BetaAppReviewDetailAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppReviewDetailAppLinkageResponse from a JSON string
beta_app_review_detail_app_linkage_response_instance = BetaAppReviewDetailAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppReviewDetailAppLinkageResponse.to_json())

# convert the object into a dict
beta_app_review_detail_app_linkage_response_dict = beta_app_review_detail_app_linkage_response_instance.to_dict()
# create an instance of BetaAppReviewDetailAppLinkageResponse from a dict
beta_app_review_detail_app_linkage_response_from_dict = BetaAppReviewDetailAppLinkageResponse.from_dict(beta_app_review_detail_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


