# BetaRecruitmentCriterionCompatibleBuildCheck


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionCompatibleBuildCheckAttributes**](BetaRecruitmentCriterionCompatibleBuildCheckAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_compatible_build_check import BetaRecruitmentCriterionCompatibleBuildCheck

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionCompatibleBuildCheck from a JSON string
beta_recruitment_criterion_compatible_build_check_instance = BetaRecruitmentCriterionCompatibleBuildCheck.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionCompatibleBuildCheck.to_json())

# convert the object into a dict
beta_recruitment_criterion_compatible_build_check_dict = beta_recruitment_criterion_compatible_build_check_instance.to_dict()
# create an instance of BetaRecruitmentCriterionCompatibleBuildCheck from a dict
beta_recruitment_criterion_compatible_build_check_from_dict = BetaRecruitmentCriterionCompatibleBuildCheck.from_dict(beta_recruitment_criterion_compatible_build_check_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


