# SubscriptionSubmissionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_submission_create_request_data import SubscriptionSubmissionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubmissionCreateRequestData from a JSON string
subscription_submission_create_request_data_instance = SubscriptionSubmissionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubmissionCreateRequestData.to_json())

# convert the object into a dict
subscription_submission_create_request_data_dict = subscription_submission_create_request_data_instance.to_dict()
# create an instance of SubscriptionSubmissionCreateRequestData from a dict
subscription_submission_create_request_data_from_dict = SubscriptionSubmissionCreateRequestData.from_dict(subscription_submission_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


