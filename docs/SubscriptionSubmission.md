# SubscriptionSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**SubscriptionAppStoreReviewScreenshotRelationships**](SubscriptionAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_submission import SubscriptionSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubmission from a JSON string
subscription_submission_instance = SubscriptionSubmission.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubmission.to_json())

# convert the object into a dict
subscription_submission_dict = subscription_submission_instance.to_dict()
# create an instance of SubscriptionSubmission from a dict
subscription_submission_from_dict = SubscriptionSubmission.from_dict(subscription_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


