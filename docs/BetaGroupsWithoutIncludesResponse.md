# BetaGroupsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaGroup]**](BetaGroup.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_groups_without_includes_response import BetaGroupsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaGroupsWithoutIncludesResponse from a JSON string
beta_groups_without_includes_response_instance = BetaGroupsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaGroupsWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_groups_without_includes_response_dict = beta_groups_without_includes_response_instance.to_dict()
# create an instance of BetaGroupsWithoutIncludesResponse from a dict
beta_groups_without_includes_response_from_dict = BetaGroupsWithoutIncludesResponse.from_dict(beta_groups_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


