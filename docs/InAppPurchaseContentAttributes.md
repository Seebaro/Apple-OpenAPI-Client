# InAppPurchaseContentAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** |  | [optional] 
**file_size** | **int** |  | [optional] 
**url** | **str** |  | [optional] 
**last_modified_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_content_attributes import InAppPurchaseContentAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseContentAttributes from a JSON string
in_app_purchase_content_attributes_instance = InAppPurchaseContentAttributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseContentAttributes.to_json())

# convert the object into a dict
in_app_purchase_content_attributes_dict = in_app_purchase_content_attributes_instance.to_dict()
# create an instance of InAppPurchaseContentAttributes from a dict
in_app_purchase_content_attributes_from_dict = InAppPurchaseContentAttributes.from_dict(in_app_purchase_content_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


