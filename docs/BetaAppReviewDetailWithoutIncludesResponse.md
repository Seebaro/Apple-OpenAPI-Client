# BetaAppReviewDetailWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaAppReviewDetail**](BetaAppReviewDetail.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_review_detail_without_includes_response import BetaAppReviewDetailWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppReviewDetailWithoutIncludesResponse from a JSON string
beta_app_review_detail_without_includes_response_instance = BetaAppReviewDetailWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppReviewDetailWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_app_review_detail_without_includes_response_dict = beta_app_review_detail_without_includes_response_instance.to_dict()
# create an instance of BetaAppReviewDetailWithoutIncludesResponse from a dict
beta_app_review_detail_without_includes_response_from_dict = BetaAppReviewDetailWithoutIncludesResponse.from_dict(beta_app_review_detail_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


