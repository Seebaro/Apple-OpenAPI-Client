# CustomerReviewsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomerReview]**](CustomerReview.md) |  | 
**included** | [**List[CustomerReviewResponseV1]**](CustomerReviewResponseV1.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_reviews_response import CustomerReviewsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewsResponse from a JSON string
customer_reviews_response_instance = CustomerReviewsResponse.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewsResponse.to_json())

# convert the object into a dict
customer_reviews_response_dict = customer_reviews_response_instance.to_dict()
# create an instance of CustomerReviewsResponse from a dict
customer_reviews_response_from_dict = CustomerReviewsResponse.from_dict(customer_reviews_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


