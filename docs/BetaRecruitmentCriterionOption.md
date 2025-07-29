# BetaRecruitmentCriterionOption


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionOptionAttributes**](BetaRecruitmentCriterionOptionAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_option import BetaRecruitmentCriterionOption

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionOption from a JSON string
beta_recruitment_criterion_option_instance = BetaRecruitmentCriterionOption.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionOption.to_json())

# convert the object into a dict
beta_recruitment_criterion_option_dict = beta_recruitment_criterion_option_instance.to_dict()
# create an instance of BetaRecruitmentCriterionOption from a dict
beta_recruitment_criterion_option_from_dict = BetaRecruitmentCriterionOption.from_dict(beta_recruitment_criterion_option_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


