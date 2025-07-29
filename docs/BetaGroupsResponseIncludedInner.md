# BetaGroupsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaRecruitmentCriterionAttributes**](BetaRecruitmentCriterionAttributes.md) |  | [optional] 
**relationships** | [**BetaTesterRelationships**](BetaTesterRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_groups_response_included_inner import BetaGroupsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of BetaGroupsResponseIncludedInner from a JSON string
beta_groups_response_included_inner_instance = BetaGroupsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(BetaGroupsResponseIncludedInner.to_json())

# convert the object into a dict
beta_groups_response_included_inner_dict = beta_groups_response_included_inner_instance.to_dict()
# create an instance of BetaGroupsResponseIncludedInner from a dict
beta_groups_response_included_inner_from_dict = BetaGroupsResponseIncludedInner.from_dict(beta_groups_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


