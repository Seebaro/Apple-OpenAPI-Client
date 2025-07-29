# SubscriptionGroupCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionGroupCreateRequestDataAttributes**](SubscriptionGroupCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_create_request_data import SubscriptionGroupCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupCreateRequestData from a JSON string
subscription_group_create_request_data_instance = SubscriptionGroupCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupCreateRequestData.to_json())

# convert the object into a dict
subscription_group_create_request_data_dict = subscription_group_create_request_data_instance.to_dict()
# create an instance of SubscriptionGroupCreateRequestData from a dict
subscription_group_create_request_data_from_dict = SubscriptionGroupCreateRequestData.from_dict(subscription_group_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


