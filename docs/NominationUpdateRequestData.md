# NominationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**NominationUpdateRequestDataAttributes**](NominationUpdateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**NominationUpdateRequestDataRelationships**](NominationUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination_update_request_data import NominationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of NominationUpdateRequestData from a JSON string
nomination_update_request_data_instance = NominationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(NominationUpdateRequestData.to_json())

# convert the object into a dict
nomination_update_request_data_dict = nomination_update_request_data_instance.to_dict()
# create an instance of NominationUpdateRequestData from a dict
nomination_update_request_data_from_dict = NominationUpdateRequestData.from_dict(nomination_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


