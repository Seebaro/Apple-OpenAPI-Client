# BetaRecruitmentCriterionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_modified_date** | **datetime** |  | [optional] 
**device_family_os_version_filters** | [**List[DeviceFamilyOsVersionFilter]**](DeviceFamilyOsVersionFilter.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_attributes import BetaRecruitmentCriterionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionAttributes from a JSON string
beta_recruitment_criterion_attributes_instance = BetaRecruitmentCriterionAttributes.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionAttributes.to_json())

# convert the object into a dict
beta_recruitment_criterion_attributes_dict = beta_recruitment_criterion_attributes_instance.to_dict()
# create an instance of BetaRecruitmentCriterionAttributes from a dict
beta_recruitment_criterion_attributes_from_dict = BetaRecruitmentCriterionAttributes.from_dict(beta_recruitment_criterion_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


