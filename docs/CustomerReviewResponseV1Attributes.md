# CustomerReviewResponseV1Attributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**response_body** | **str** |  | [optional] 
**last_modified_date** | **datetime** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_response_v1_attributes import CustomerReviewResponseV1Attributes

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1Attributes from a JSON string
customer_review_response_v1_attributes_instance = CustomerReviewResponseV1Attributes.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1Attributes.to_json())

# convert the object into a dict
customer_review_response_v1_attributes_dict = customer_review_response_v1_attributes_instance.to_dict()
# create an instance of CustomerReviewResponseV1Attributes from a dict
customer_review_response_v1_attributes_from_dict = CustomerReviewResponseV1Attributes.from_dict(customer_review_response_v1_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


