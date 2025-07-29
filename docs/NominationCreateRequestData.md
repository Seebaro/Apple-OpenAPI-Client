# NominationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**NominationCreateRequestDataAttributes**](NominationCreateRequestDataAttributes.md) |  | 
**relationships** | [**NominationCreateRequestDataRelationships**](NominationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.nomination_create_request_data import NominationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of NominationCreateRequestData from a JSON string
nomination_create_request_data_instance = NominationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(NominationCreateRequestData.to_json())

# convert the object into a dict
nomination_create_request_data_dict = nomination_create_request_data_instance.to_dict()
# create an instance of NominationCreateRequestData from a dict
nomination_create_request_data_from_dict = NominationCreateRequestData.from_dict(nomination_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


