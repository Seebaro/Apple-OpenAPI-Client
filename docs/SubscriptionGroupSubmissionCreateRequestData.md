# SubscriptionGroupSubmissionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**SubscriptionGroupLocalizationCreateRequestDataRelationships**](SubscriptionGroupLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_submission_create_request_data import SubscriptionGroupSubmissionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubmissionCreateRequestData from a JSON string
subscription_group_submission_create_request_data_instance = SubscriptionGroupSubmissionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubmissionCreateRequestData.to_json())

# convert the object into a dict
subscription_group_submission_create_request_data_dict = subscription_group_submission_create_request_data_instance.to_dict()
# create an instance of SubscriptionGroupSubmissionCreateRequestData from a dict
subscription_group_submission_create_request_data_from_dict = SubscriptionGroupSubmissionCreateRequestData.from_dict(subscription_group_submission_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


