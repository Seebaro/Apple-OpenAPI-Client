# CustomerReviewResponseV1Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomerReviewResponseV1**](CustomerReviewResponseV1.md) |  | 
**included** | [**List[CustomerReview]**](CustomerReview.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.customer_review_response_v1_response import CustomerReviewResponseV1Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1Response from a JSON string
customer_review_response_v1_response_instance = CustomerReviewResponseV1Response.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1Response.to_json())

# convert the object into a dict
customer_review_response_v1_response_dict = customer_review_response_v1_response_instance.to_dict()
# create an instance of CustomerReviewResponseV1Response from a dict
customer_review_response_v1_response_from_dict = CustomerReviewResponseV1Response.from_dict(customer_review_response_v1_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


