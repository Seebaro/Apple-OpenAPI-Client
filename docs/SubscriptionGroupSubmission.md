# SubscriptionGroupSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_submission import SubscriptionGroupSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubmission from a JSON string
subscription_group_submission_instance = SubscriptionGroupSubmission.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubmission.to_json())

# convert the object into a dict
subscription_group_submission_dict = subscription_group_submission_instance.to_dict()
# create an instance of SubscriptionGroupSubmission from a dict
subscription_group_submission_from_dict = SubscriptionGroupSubmission.from_dict(subscription_group_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


