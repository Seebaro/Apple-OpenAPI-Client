# TerritoriesWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Territory]**](Territory.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.territories_without_includes_response import TerritoriesWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoriesWithoutIncludesResponse from a JSON string
territories_without_includes_response_instance = TerritoriesWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(TerritoriesWithoutIncludesResponse.to_json())

# convert the object into a dict
territories_without_includes_response_dict = territories_without_includes_response_instance.to_dict()
# create an instance of TerritoriesWithoutIncludesResponse from a dict
territories_without_includes_response_from_dict = TerritoriesWithoutIncludesResponse.from_dict(territories_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


