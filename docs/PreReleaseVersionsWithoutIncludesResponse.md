# PreReleaseVersionsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PrereleaseVersion]**](PrereleaseVersion.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.pre_release_versions_without_includes_response import PreReleaseVersionsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PreReleaseVersionsWithoutIncludesResponse from a JSON string
pre_release_versions_without_includes_response_instance = PreReleaseVersionsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(PreReleaseVersionsWithoutIncludesResponse.to_json())

# convert the object into a dict
pre_release_versions_without_includes_response_dict = pre_release_versions_without_includes_response_instance.to_dict()
# create an instance of PreReleaseVersionsWithoutIncludesResponse from a dict
pre_release_versions_without_includes_response_from_dict = PreReleaseVersionsWithoutIncludesResponse.from_dict(pre_release_versions_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


