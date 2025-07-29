# BuildsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Build]**](Build.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.builds_without_includes_response import BuildsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildsWithoutIncludesResponse from a JSON string
builds_without_includes_response_instance = BuildsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildsWithoutIncludesResponse.to_json())

# convert the object into a dict
builds_without_includes_response_dict = builds_without_includes_response_instance.to_dict()
# create an instance of BuildsWithoutIncludesResponse from a dict
builds_without_includes_response_from_dict = BuildsWithoutIncludesResponse.from_dict(builds_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


