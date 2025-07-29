# SubscriptionSubmissionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionSubmissionCreateRequestData**](SubscriptionSubmissionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_submission_create_request import SubscriptionSubmissionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubmissionCreateRequest from a JSON string
subscription_submission_create_request_instance = SubscriptionSubmissionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubmissionCreateRequest.to_json())

# convert the object into a dict
subscription_submission_create_request_dict = subscription_submission_create_request_instance.to_dict()
# create an instance of SubscriptionSubmissionCreateRequest from a dict
subscription_submission_create_request_from_dict = SubscriptionSubmissionCreateRequest.from_dict(subscription_submission_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


