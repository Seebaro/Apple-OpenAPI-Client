# BetaTestersResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BuildAttributes**](BuildAttributes.md) |  | [optional] 
**relationships** | [**BuildRelationships**](BuildRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_testers_response_included_inner import BetaTestersResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of BetaTestersResponseIncludedInner from a JSON string
beta_testers_response_included_inner_instance = BetaTestersResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(BetaTestersResponseIncludedInner.to_json())

# convert the object into a dict
beta_testers_response_included_inner_dict = beta_testers_response_included_inner_instance.to_dict()
# create an instance of BetaTestersResponseIncludedInner from a dict
beta_testers_response_included_inner_from_dict = BetaTestersResponseIncludedInner.from_dict(beta_testers_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


