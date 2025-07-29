# NominationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAttributes**](TerritoryAttributes.md) |  | [optional] 
**relationships** | [**AppEventRelationships**](AppEventRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.nominations_response_included_inner import NominationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of NominationsResponseIncludedInner from a JSON string
nominations_response_included_inner_instance = NominationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(NominationsResponseIncludedInner.to_json())

# convert the object into a dict
nominations_response_included_inner_dict = nominations_response_included_inner_instance.to_dict()
# create an instance of NominationsResponseIncludedInner from a dict
nominations_response_included_inner_from_dict = NominationsResponseIncludedInner.from_dict(nominations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


