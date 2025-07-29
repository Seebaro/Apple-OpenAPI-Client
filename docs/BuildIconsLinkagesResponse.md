# BuildIconsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BuildRelationshipsIconsDataInner]**](BuildRelationshipsIconsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_icons_linkages_response import BuildIconsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildIconsLinkagesResponse from a JSON string
build_icons_linkages_response_instance = BuildIconsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildIconsLinkagesResponse.to_json())

# convert the object into a dict
build_icons_linkages_response_dict = build_icons_linkages_response_instance.to_dict()
# create an instance of BuildIconsLinkagesResponse from a dict
build_icons_linkages_response_from_dict = BuildIconsLinkagesResponse.from_dict(build_icons_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


