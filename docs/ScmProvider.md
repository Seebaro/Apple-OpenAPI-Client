# ScmProvider


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ScmProviderAttributes**](ScmProviderAttributes.md) |  | [optional] 
**relationships** | [**ScmProviderRelationships**](ScmProviderRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_provider import ScmProvider

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProvider from a JSON string
scm_provider_instance = ScmProvider.from_json(json)
# print the JSON string representation of the object
print(ScmProvider.to_json())

# convert the object into a dict
scm_provider_dict = scm_provider_instance.to_dict()
# create an instance of ScmProvider from a dict
scm_provider_from_dict = ScmProvider.from_dict(scm_provider_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


