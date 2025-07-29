# NominationUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**NominationUpdateRequestData**](NominationUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.nomination_update_request import NominationUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of NominationUpdateRequest from a JSON string
nomination_update_request_instance = NominationUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(NominationUpdateRequest.to_json())

# convert the object into a dict
nomination_update_request_dict = nomination_update_request_instance.to_dict()
# create an instance of NominationUpdateRequest from a dict
nomination_update_request_from_dict = NominationUpdateRequest.from_dict(nomination_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


