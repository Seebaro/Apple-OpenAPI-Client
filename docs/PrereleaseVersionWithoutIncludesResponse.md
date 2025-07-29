# PrereleaseVersionWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PrereleaseVersion**](PrereleaseVersion.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.prerelease_version_without_includes_response import PrereleaseVersionWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PrereleaseVersionWithoutIncludesResponse from a JSON string
prerelease_version_without_includes_response_instance = PrereleaseVersionWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(PrereleaseVersionWithoutIncludesResponse.to_json())

# convert the object into a dict
prerelease_version_without_includes_response_dict = prerelease_version_without_includes_response_instance.to_dict()
# create an instance of PrereleaseVersionWithoutIncludesResponse from a dict
prerelease_version_without_includes_response_from_dict = PrereleaseVersionWithoutIncludesResponse.from_dict(prerelease_version_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


