# AppStoreVersionAppStoreVersionSubmissionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionRelationshipsAppStoreVersionSubmissionData**](AppStoreVersionRelationshipsAppStoreVersionSubmissionData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_app_store_version_submission_linkage_response import AppStoreVersionAppStoreVersionSubmissionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionAppStoreVersionSubmissionLinkageResponse from a JSON string
app_store_version_app_store_version_submission_linkage_response_instance = AppStoreVersionAppStoreVersionSubmissionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionAppStoreVersionSubmissionLinkageResponse.to_json())

# convert the object into a dict
app_store_version_app_store_version_submission_linkage_response_dict = app_store_version_app_store_version_submission_linkage_response_instance.to_dict()
# create an instance of AppStoreVersionAppStoreVersionSubmissionLinkageResponse from a dict
app_store_version_app_store_version_submission_linkage_response_from_dict = AppStoreVersionAppStoreVersionSubmissionLinkageResponse.from_dict(app_store_version_app_store_version_submission_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


