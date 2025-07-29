# ActorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**Actor**](Actor.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.actor_response import ActorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ActorResponse from a JSON string
actor_response_instance = ActorResponse.from_json(json)
# print the JSON string representation of the object
print(ActorResponse.to_json())

# convert the object into a dict
actor_response_dict = actor_response_instance.to_dict()
# create an instance of ActorResponse from a dict
actor_response_from_dict = ActorResponse.from_dict(actor_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


