# BuildsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BuildBundleAttributes**](BuildBundleAttributes.md) |  | [optional] 
**relationships** | [**BuildBundleRelationships**](BuildBundleRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.builds_response_included_inner import BuildsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of BuildsResponseIncludedInner from a JSON string
builds_response_included_inner_instance = BuildsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(BuildsResponseIncludedInner.to_json())

# convert the object into a dict
builds_response_included_inner_dict = builds_response_included_inner_instance.to_dict()
# create an instance of BuildsResponseIncludedInner from a dict
builds_response_included_inner_from_dict = BuildsResponseIncludedInner.from_dict(builds_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


