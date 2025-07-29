# BuildWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**Build**](Build.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_without_includes_response import BuildWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildWithoutIncludesResponse from a JSON string
build_without_includes_response_instance = BuildWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildWithoutIncludesResponse.to_json())

# convert the object into a dict
build_without_includes_response_dict = build_without_includes_response_instance.to_dict()
# create an instance of BuildWithoutIncludesResponse from a dict
build_without_includes_response_from_dict = BuildWithoutIncludesResponse.from_dict(build_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


