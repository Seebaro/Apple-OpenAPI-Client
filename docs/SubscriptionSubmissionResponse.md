# SubscriptionSubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionSubmission**](SubscriptionSubmission.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_submission_response import SubscriptionSubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubmissionResponse from a JSON string
subscription_submission_response_instance = SubscriptionSubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubmissionResponse.to_json())

# convert the object into a dict
subscription_submission_response_dict = subscription_submission_response_instance.to_dict()
# create an instance of SubscriptionSubmissionResponse from a dict
subscription_submission_response_from_dict = SubscriptionSubmissionResponse.from_dict(subscription_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


