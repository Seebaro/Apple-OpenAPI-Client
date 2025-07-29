# SubscriptionGroupSubmissionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroupSubmissionCreateRequestData**](SubscriptionGroupSubmissionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_submission_create_request import SubscriptionGroupSubmissionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubmissionCreateRequest from a JSON string
subscription_group_submission_create_request_instance = SubscriptionGroupSubmissionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubmissionCreateRequest.to_json())

# convert the object into a dict
subscription_group_submission_create_request_dict = subscription_group_submission_create_request_instance.to_dict()
# create an instance of SubscriptionGroupSubmissionCreateRequest from a dict
subscription_group_submission_create_request_from_dict = SubscriptionGroupSubmissionCreateRequest.from_dict(subscription_group_submission_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


