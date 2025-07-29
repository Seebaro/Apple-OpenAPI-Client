# PassTypeId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**MerchantIdAttributes**](MerchantIdAttributes.md) |  | [optional] 
**relationships** | [**MerchantIdRelationships**](MerchantIdRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.pass_type_id import PassTypeId

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeId from a JSON string
pass_type_id_instance = PassTypeId.from_json(json)
# print the JSON string representation of the object
print(PassTypeId.to_json())

# convert the object into a dict
pass_type_id_dict = pass_type_id_instance.to_dict()
# create an instance of PassTypeId from a dict
pass_type_id_from_dict = PassTypeId.from_dict(pass_type_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


