# BetaRecruitmentCriterionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaRecruitmentCriterion**](BetaRecruitmentCriterion.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_response import BetaRecruitmentCriterionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionResponse from a JSON string
beta_recruitment_criterion_response_instance = BetaRecruitmentCriterionResponse.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionResponse.to_json())

# convert the object into a dict
beta_recruitment_criterion_response_dict = beta_recruitment_criterion_response_instance.to_dict()
# create an instance of BetaRecruitmentCriterionResponse from a dict
beta_recruitment_criterion_response_from_dict = BetaRecruitmentCriterionResponse.from_dict(beta_recruitment_criterion_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


