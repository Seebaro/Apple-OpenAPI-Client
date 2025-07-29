# ScmProviderType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**is_on_premise** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.scm_provider_type import ScmProviderType

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProviderType from a JSON string
scm_provider_type_instance = ScmProviderType.from_json(json)
# print the JSON string representation of the object
print(ScmProviderType.to_json())

# convert the object into a dict
scm_provider_type_dict = scm_provider_type_instance.to_dict()
# create an instance of ScmProviderType from a dict
scm_provider_type_from_dict = ScmProviderType.from_dict(scm_provider_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


