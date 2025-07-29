# ScmProviderResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ScmProvider**](ScmProvider.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.scm_provider_response import ScmProviderResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProviderResponse from a JSON string
scm_provider_response_instance = ScmProviderResponse.from_json(json)
# print the JSON string representation of the object
print(ScmProviderResponse.to_json())

# convert the object into a dict
scm_provider_response_dict = scm_provider_response_instance.to_dict()
# create an instance of ScmProviderResponse from a dict
scm_provider_response_from_dict = ScmProviderResponse.from_dict(scm_provider_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


