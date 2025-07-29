# CustomerReviewResponseV1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CustomerReviewResponseV1Attributes**](CustomerReviewResponseV1Attributes.md) |  | [optional] 
**relationships** | [**CustomerReviewResponseV1Relationships**](CustomerReviewResponseV1Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_response_v1 import CustomerReviewResponseV1

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1 from a JSON string
customer_review_response_v1_instance = CustomerReviewResponseV1.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1.to_json())

# convert the object into a dict
customer_review_response_v1_dict = customer_review_response_v1_instance.to_dict()
# create an instance of CustomerReviewResponseV1 from a dict
customer_review_response_v1_from_dict = CustomerReviewResponseV1.from_dict(customer_review_response_v1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


