# InAppPurchaseSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotRelationships**](InAppPurchaseAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_submission import InAppPurchaseSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseSubmission from a JSON string
in_app_purchase_submission_instance = InAppPurchaseSubmission.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseSubmission.to_json())

# convert the object into a dict
in_app_purchase_submission_dict = in_app_purchase_submission_instance.to_dict()
# create an instance of InAppPurchaseSubmission from a dict
in_app_purchase_submission_from_dict = InAppPurchaseSubmission.from_dict(in_app_purchase_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


