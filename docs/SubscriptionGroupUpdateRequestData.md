# SubscriptionGroupUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterGroupAttributes**](GameCenterGroupAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_update_request_data import SubscriptionGroupUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupUpdateRequestData from a JSON string
subscription_group_update_request_data_instance = SubscriptionGroupUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupUpdateRequestData.to_json())

# convert the object into a dict
subscription_group_update_request_data_dict = subscription_group_update_request_data_instance.to_dict()
# create an instance of SubscriptionGroupUpdateRequestData from a dict
subscription_group_update_request_data_from_dict = SubscriptionGroupUpdateRequestData.from_dict(subscription_group_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


