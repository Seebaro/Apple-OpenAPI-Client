# BetaRecruitmentCriterionUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionUpdateRequestDataAttributes**](BetaRecruitmentCriterionUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_recruitment_criterion_update_request_data import BetaRecruitmentCriterionUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BetaRecruitmentCriterionUpdateRequestData from a JSON string
beta_recruitment_criterion_update_request_data_instance = BetaRecruitmentCriterionUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(BetaRecruitmentCriterionUpdateRequestData.to_json())

# convert the object into a dict
beta_recruitment_criterion_update_request_data_dict = beta_recruitment_criterion_update_request_data_instance.to_dict()
# create an instance of BetaRecruitmentCriterionUpdateRequestData from a dict
beta_recruitment_criterion_update_request_data_from_dict = BetaRecruitmentCriterionUpdateRequestData.from_dict(beta_recruitment_criterion_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


