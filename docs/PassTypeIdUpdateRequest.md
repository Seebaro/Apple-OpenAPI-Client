# PassTypeIdUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PassTypeIdUpdateRequestData**](PassTypeIdUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.pass_type_id_update_request import PassTypeIdUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdUpdateRequest from a JSON string
pass_type_id_update_request_instance = PassTypeIdUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdUpdateRequest.to_json())

# convert the object into a dict
pass_type_id_update_request_dict = pass_type_id_update_request_instance.to_dict()
# create an instance of PassTypeIdUpdateRequest from a dict
pass_type_id_update_request_from_dict = PassTypeIdUpdateRequest.from_dict(pass_type_id_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


