# BuildIconsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BuildIcon]**](BuildIcon.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_icons_without_includes_response import BuildIconsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildIconsWithoutIncludesResponse from a JSON string
build_icons_without_includes_response_instance = BuildIconsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildIconsWithoutIncludesResponse.to_json())

# convert the object into a dict
build_icons_without_includes_response_dict = build_icons_without_includes_response_instance.to_dict()
# create an instance of BuildIconsWithoutIncludesResponse from a dict
build_icons_without_includes_response_from_dict = BuildIconsWithoutIncludesResponse.from_dict(build_icons_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


