# BetaRecruitmentCriterionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaRecruitmentCriterionCreateRequestData**](BetaRecruitmentCriterionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_create_request import BetaRecruitmentCriterionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionCreateRequest from a JSON string
beta_recruitment_criterion_create_request_instance = BetaRecruitmentCriterionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionCreateRequest.to_json())

# convert the object into a dict
beta_recruitment_criterion_create_request_dict = beta_recruitment_criterion_create_request_instance.to_dict()
# create an instance of BetaRecruitmentCriterionCreateRequest from a dict
beta_recruitment_criterion_create_request_from_dict = BetaRecruitmentCriterionCreateRequest.from_dict(beta_recruitment_criterion_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


