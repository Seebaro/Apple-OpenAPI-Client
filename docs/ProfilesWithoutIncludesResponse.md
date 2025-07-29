# ProfilesWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Profile]**](Profile.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.profiles_without_includes_response import ProfilesWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfilesWithoutIncludesResponse from a JSON string
profiles_without_includes_response_instance = ProfilesWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(ProfilesWithoutIncludesResponse.to_json())

# convert the object into a dict
profiles_without_includes_response_dict = profiles_without_includes_response_instance.to_dict()
# create an instance of ProfilesWithoutIncludesResponse from a dict
profiles_without_includes_response_from_dict = ProfilesWithoutIncludesResponse.from_dict(profiles_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


