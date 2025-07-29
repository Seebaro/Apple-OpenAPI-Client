# AppBetaAppReviewDetailLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsBetaAppReviewDetailData**](AppRelationshipsBetaAppReviewDetailData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_beta_app_review_detail_linkage_response import AppBetaAppReviewDetailLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppBetaAppReviewDetailLinkageResponse from a JSON string
app_beta_app_review_detail_linkage_response_instance = AppBetaAppReviewDetailLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppBetaAppReviewDetailLinkageResponse.to_json())

# convert the object into a dict
app_beta_app_review_detail_linkage_response_dict = app_beta_app_review_detail_linkage_response_instance.to_dict()
# create an instance of AppBetaAppReviewDetailLinkageResponse from a dict
app_beta_app_review_detail_linkage_response_from_dict = AppBetaAppReviewDetailLinkageResponse.from_dict(app_beta_app_review_detail_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


