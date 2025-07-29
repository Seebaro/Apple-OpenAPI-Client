# Nomination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**NominationAttributes**](NominationAttributes.md) |  | [optional] 
**relationships** | [**NominationRelationships**](NominationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination import Nomination

# TODO update the JSON string below
json = "{}"
# create an instance of Nomination from a JSON string
nomination_instance = Nomination.from_json(json)
# print the JSON string representation of the object
print(Nomination.to_json())

# convert the object into a dict
nomination_dict = nomination_instance.to_dict()
# create an instance of Nomination from a dict
nomination_from_dict = Nomination.from_dict(nomination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


