# AppStoreVersionCustomerReviewsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomerReviewResponseV1RelationshipsReviewData]**](CustomerReviewResponseV1RelationshipsReviewData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_customer_reviews_linkages_response import AppStoreVersionCustomerReviewsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionCustomerReviewsLinkagesResponse from a JSON string
app_store_version_customer_reviews_linkages_response_instance = AppStoreVersionCustomerReviewsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionCustomerReviewsLinkagesResponse.to_json())

# convert the object into a dict
app_store_version_customer_reviews_linkages_response_dict = app_store_version_customer_reviews_linkages_response_instance.to_dict()
# create an instance of AppStoreVersionCustomerReviewsLinkagesResponse from a dict
app_store_version_customer_reviews_linkages_response_from_dict = AppStoreVersionCustomerReviewsLinkagesResponse.from_dict(app_store_version_customer_reviews_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


