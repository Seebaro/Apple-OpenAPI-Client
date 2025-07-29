# ActorsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Actor]**](Actor.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.actors_response import ActorsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ActorsResponse from a JSON string
actors_response_instance = ActorsResponse.from_json(json)
# print the JSON string representation of the object
print(ActorsResponse.to_json())

# convert the object into a dict
actors_response_dict = actors_response_instance.to_dict()
# create an instance of ActorsResponse from a dict
actors_response_from_dict = ActorsResponse.from_dict(actors_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


