# PassTypeIdsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PassTypeId]**](PassTypeId.md) |  | 
**included** | [**List[Certificate]**](Certificate.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.pass_type_ids_response import PassTypeIdsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdsResponse from a JSON string
pass_type_ids_response_instance = PassTypeIdsResponse.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdsResponse.to_json())

# convert the object into a dict
pass_type_ids_response_dict = pass_type_ids_response_instance.to_dict()
# create an instance of PassTypeIdsResponse from a dict
pass_type_ids_response_from_dict = PassTypeIdsResponse.from_dict(pass_type_ids_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


