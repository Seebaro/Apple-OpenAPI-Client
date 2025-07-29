# BetaRecruitmentCriterionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionCreateRequestDataAttributes**](BetaRecruitmentCriterionCreateRequestDataAttributes.md) |  | 
**relationships** | [**BetaRecruitmentCriterionCreateRequestDataRelationships**](BetaRecruitmentCriterionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_create_request_data import BetaRecruitmentCriterionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionCreateRequestData from a JSON string
beta_recruitment_criterion_create_request_data_instance = BetaRecruitmentCriterionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionCreateRequestData.to_json())

# convert the object into a dict
beta_recruitment_criterion_create_request_data_dict = beta_recruitment_criterion_create_request_data_instance.to_dict()
# create an instance of BetaRecruitmentCriterionCreateRequestData from a dict
beta_recruitment_criterion_create_request_data_from_dict = BetaRecruitmentCriterionCreateRequestData.from_dict(beta_recruitment_criterion_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


