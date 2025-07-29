# BetaRecruitmentCriterion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionAttributes**](BetaRecruitmentCriterionAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_recruitment_criterion import BetaRecruitmentCriterion

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterion from a JSON string
beta_recruitment_criterion_instance = BetaRecruitmentCriterion.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterion.to_json())

# convert the object into a dict
beta_recruitment_criterion_dict = beta_recruitment_criterion_instance.to_dict()
# create an instance of BetaRecruitmentCriterion from a dict
beta_recruitment_criterion_from_dict = BetaRecruitmentCriterion.from_dict(beta_recruitment_criterion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


