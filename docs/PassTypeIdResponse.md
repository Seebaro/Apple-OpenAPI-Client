# PassTypeIdResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PassTypeId**](PassTypeId.md) |  | 
**included** | [**List[Certificate]**](Certificate.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.pass_type_id_response import PassTypeIdResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdResponse from a JSON string
pass_type_id_response_instance = PassTypeIdResponse.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdResponse.to_json())

# convert the object into a dict
pass_type_id_response_dict = pass_type_id_response_instance.to_dict()
# create an instance of PassTypeIdResponse from a dict
pass_type_id_response_from_dict = PassTypeIdResponse.from_dict(pass_type_id_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


