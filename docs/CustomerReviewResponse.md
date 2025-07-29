# CustomerReviewResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomerReview**](CustomerReview.md) |  | 
**included** | [**List[CustomerReviewResponseV1]**](CustomerReviewResponseV1.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.customer_review_response import CustomerReviewResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponse from a JSON string
customer_review_response_instance = CustomerReviewResponse.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponse.to_json())

# convert the object into a dict
customer_review_response_dict = customer_review_response_instance.to_dict()
# create an instance of CustomerReviewResponse from a dict
customer_review_response_from_dict = CustomerReviewResponse.from_dict(customer_review_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


