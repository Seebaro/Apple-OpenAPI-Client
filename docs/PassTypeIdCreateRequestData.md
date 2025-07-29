# PassTypeIdCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**MerchantIdCreateRequestDataAttributes**](MerchantIdCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.pass_type_id_create_request_data import PassTypeIdCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdCreateRequestData from a JSON string
pass_type_id_create_request_data_instance = PassTypeIdCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdCreateRequestData.to_json())

# convert the object into a dict
pass_type_id_create_request_data_dict = pass_type_id_create_request_data_instance.to_dict()
# create an instance of PassTypeIdCreateRequestData from a dict
pass_type_id_create_request_data_from_dict = PassTypeIdCreateRequestData.from_dict(pass_type_id_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


