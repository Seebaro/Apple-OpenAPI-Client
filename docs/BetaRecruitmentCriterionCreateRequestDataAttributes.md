# BetaRecruitmentCriterionCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_family_os_version_filters** | [**List[DeviceFamilyOsVersionFilter]**](DeviceFamilyOsVersionFilter.md) |  | 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_create_request_data_attributes import BetaRecruitmentCriterionCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionCreateRequestDataAttributes from a JSON string
beta_recruitment_criterion_create_request_data_attributes_instance = BetaRecruitmentCriterionCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionCreateRequestDataAttributes.to_json())

# convert the object into a dict
beta_recruitment_criterion_create_request_data_attributes_dict = beta_recruitment_criterion_create_request_data_attributes_instance.to_dict()
# create an instance of BetaRecruitmentCriterionCreateRequestDataAttributes from a dict
beta_recruitment_criterion_create_request_data_attributes_from_dict = BetaRecruitmentCriterionCreateRequestDataAttributes.from_dict(beta_recruitment_criterion_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


