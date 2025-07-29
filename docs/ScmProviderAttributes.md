# ScmProviderAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scm_provider_type** | [**ScmProviderType**](ScmProviderType.md) |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.scm_provider_attributes import ScmProviderAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProviderAttributes from a JSON string
scm_provider_attributes_instance = ScmProviderAttributes.from_json(json)
# print the JSON string representation of the object
print(ScmProviderAttributes.to_json())

# convert the object into a dict
scm_provider_attributes_dict = scm_provider_attributes_instance.to_dict()
# create an instance of ScmProviderAttributes from a dict
scm_provider_attributes_from_dict = ScmProviderAttributes.from_dict(scm_provider_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


