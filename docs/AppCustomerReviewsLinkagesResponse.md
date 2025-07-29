# AppCustomerReviewsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomerReviewResponseV1RelationshipsReviewData]**](CustomerReviewResponseV1RelationshipsReviewData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_customer_reviews_linkages_response import AppCustomerReviewsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomerReviewsLinkagesResponse from a JSON string
app_customer_reviews_linkages_response_instance = AppCustomerReviewsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCustomerReviewsLinkagesResponse.to_json())

# convert the object into a dict
app_customer_reviews_linkages_response_dict = app_customer_reviews_linkages_response_instance.to_dict()
# create an instance of AppCustomerReviewsLinkagesResponse from a dict
app_customer_reviews_linkages_response_from_dict = AppCustomerReviewsLinkagesResponse.from_dict(app_customer_reviews_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


