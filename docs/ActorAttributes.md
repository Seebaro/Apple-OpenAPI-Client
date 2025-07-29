# ActorAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**actor_type** | **str** |  | [optional] 
**user_first_name** | **str** |  | [optional] 
**user_last_name** | **str** |  | [optional] 
**user_email** | **str** |  | [optional] 
**api_key_id** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.actor_attributes import ActorAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ActorAttributes from a JSON string
actor_attributes_instance = ActorAttributes.from_json(json)
# print the JSON string representation of the object
print(ActorAttributes.to_json())

# convert the object into a dict
actor_attributes_dict = actor_attributes_instance.to_dict()
# create an instance of ActorAttributes from a dict
actor_attributes_from_dict = ActorAttributes.from_dict(actor_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


