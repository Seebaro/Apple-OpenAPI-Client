# InAppPurchaseSubmissionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseSubmissionCreateRequestData**](InAppPurchaseSubmissionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_submission_create_request import InAppPurchaseSubmissionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseSubmissionCreateRequest from a JSON string
in_app_purchase_submission_create_request_instance = InAppPurchaseSubmissionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseSubmissionCreateRequest.to_json())

# convert the object into a dict
in_app_purchase_submission_create_request_dict = in_app_purchase_submission_create_request_instance.to_dict()
# create an instance of InAppPurchaseSubmissionCreateRequest from a dict
in_app_purchase_submission_create_request_from_dict = InAppPurchaseSubmissionCreateRequest.from_dict(in_app_purchase_submission_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


