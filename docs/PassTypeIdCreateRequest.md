# PassTypeIdCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PassTypeIdCreateRequestData**](PassTypeIdCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.pass_type_id_create_request import PassTypeIdCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdCreateRequest from a JSON string
pass_type_id_create_request_instance = PassTypeIdCreateRequest.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdCreateRequest.to_json())

# convert the object into a dict
pass_type_id_create_request_dict = pass_type_id_create_request_instance.to_dict()
# create an instance of PassTypeIdCreateRequest from a dict
pass_type_id_create_request_from_dict = PassTypeIdCreateRequest.from_dict(pass_type_id_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


