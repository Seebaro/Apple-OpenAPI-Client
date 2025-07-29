# NominationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**NominationCreateRequestData**](NominationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.nomination_create_request import NominationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of NominationCreateRequest from a JSON string
nomination_create_request_instance = NominationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(NominationCreateRequest.to_json())

# convert the object into a dict
nomination_create_request_dict = nomination_create_request_instance.to_dict()
# create an instance of NominationCreateRequest from a dict
nomination_create_request_from_dict = NominationCreateRequest.from_dict(nomination_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


