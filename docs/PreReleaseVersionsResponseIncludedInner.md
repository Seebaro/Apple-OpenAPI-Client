# PreReleaseVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppAttributes**](AppAttributes.md) |  | [optional] 
**relationships** | [**AppRelationships**](AppRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.pre_release_versions_response_included_inner import PreReleaseVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of PreReleaseVersionsResponseIncludedInner from a JSON string
pre_release_versions_response_included_inner_instance = PreReleaseVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(PreReleaseVersionsResponseIncludedInner.to_json())

# convert the object into a dict
pre_release_versions_response_included_inner_dict = pre_release_versions_response_included_inner_instance.to_dict()
# create an instance of PreReleaseVersionsResponseIncludedInner from a dict
pre_release_versions_response_included_inner_from_dict = PreReleaseVersionsResponseIncludedInner.from_dict(pre_release_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


