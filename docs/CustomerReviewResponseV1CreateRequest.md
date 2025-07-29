# CustomerReviewResponseV1CreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomerReviewResponseV1CreateRequestData**](CustomerReviewResponseV1CreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.customer_review_response_v1_create_request import CustomerReviewResponseV1CreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1CreateRequest from a JSON string
customer_review_response_v1_create_request_instance = CustomerReviewResponseV1CreateRequest.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1CreateRequest.to_json())

# convert the object into a dict
customer_review_response_v1_create_request_dict = customer_review_response_v1_create_request_instance.to_dict()
# create an instance of CustomerReviewResponseV1CreateRequest from a dict
customer_review_response_v1_create_request_from_dict = CustomerReviewResponseV1CreateRequest.from_dict(customer_review_response_v1_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


