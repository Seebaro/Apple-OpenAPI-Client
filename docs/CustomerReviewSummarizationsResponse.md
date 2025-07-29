# CustomerReviewSummarizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomerReviewSummarization]**](CustomerReviewSummarization.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_summarizations_response import CustomerReviewSummarizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewSummarizationsResponse from a JSON string
customer_review_summarizations_response_instance = CustomerReviewSummarizationsResponse.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewSummarizationsResponse.to_json())

# convert the object into a dict
customer_review_summarizations_response_dict = customer_review_summarizations_response_instance.to_dict()
# create an instance of CustomerReviewSummarizationsResponse from a dict
customer_review_summarizations_response_from_dict = CustomerReviewSummarizationsResponse.from_dict(customer_review_summarizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


