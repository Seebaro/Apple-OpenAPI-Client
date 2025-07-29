# BetaRecruitmentCriterionUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaRecruitmentCriterionUpdateRequestData**](BetaRecruitmentCriterionUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_update_request import BetaRecruitmentCriterionUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionUpdateRequest from a JSON string
beta_recruitment_criterion_update_request_instance = BetaRecruitmentCriterionUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionUpdateRequest.to_json())

# convert the object into a dict
beta_recruitment_criterion_update_request_dict = beta_recruitment_criterion_update_request_instance.to_dict()
# create an instance of BetaRecruitmentCriterionUpdateRequest from a dict
beta_recruitment_criterion_update_request_from_dict = BetaRecruitmentCriterionUpdateRequest.from_dict(beta_recruitment_criterion_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


