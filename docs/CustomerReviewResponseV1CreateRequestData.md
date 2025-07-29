# CustomerReviewResponseV1CreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**CustomerReviewResponseV1CreateRequestDataAttributes**](CustomerReviewResponseV1CreateRequestDataAttributes.md) |  | 
**relationships** | [**CustomerReviewResponseV1CreateRequestDataRelationships**](CustomerReviewResponseV1CreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.customer_review_response_v1_create_request_data import CustomerReviewResponseV1CreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1CreateRequestData from a JSON string
customer_review_response_v1_create_request_data_instance = CustomerReviewResponseV1CreateRequestData.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1CreateRequestData.to_json())

# convert the object into a dict
customer_review_response_v1_create_request_data_dict = customer_review_response_v1_create_request_data_instance.to_dict()
# create an instance of CustomerReviewResponseV1CreateRequestData from a dict
customer_review_response_v1_create_request_data_from_dict = CustomerReviewResponseV1CreateRequestData.from_dict(customer_review_response_v1_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


