# SubscriptionGroupSubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroupSubmission**](SubscriptionGroupSubmission.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_submission_response import SubscriptionGroupSubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubmissionResponse from a JSON string
subscription_group_submission_response_instance = SubscriptionGroupSubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubmissionResponse.to_json())

# convert the object into a dict
subscription_group_submission_response_dict = subscription_group_submission_response_instance.to_dict()
# create an instance of SubscriptionGroupSubmissionResponse from a dict
subscription_group_submission_response_from_dict = SubscriptionGroupSubmissionResponse.from_dict(subscription_group_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


