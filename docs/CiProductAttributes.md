# CiProductAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**product_type** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_product_attributes import CiProductAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductAttributes from a JSON string
ci_product_attributes_instance = CiProductAttributes.from_json(json)
# print the JSON string representation of the object
print(CiProductAttributes.to_json())

# convert the object into a dict
ci_product_attributes_dict = ci_product_attributes_instance.to_dict()
# create an instance of CiProductAttributes from a dict
ci_product_attributes_from_dict = CiProductAttributes.from_dict(ci_product_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


