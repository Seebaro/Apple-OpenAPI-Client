# PassTypeIdUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BundleIdUpdateRequestDataAttributes**](BundleIdUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.pass_type_id_update_request_data import PassTypeIdUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdUpdateRequestData from a JSON string
pass_type_id_update_request_data_instance = PassTypeIdUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdUpdateRequestData.to_json())

# convert the object into a dict
pass_type_id_update_request_data_dict = pass_type_id_update_request_data_instance.to_dict()
# create an instance of PassTypeIdUpdateRequestData from a dict
pass_type_id_update_request_data_from_dict = PassTypeIdUpdateRequestData.from_dict(pass_type_id_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


