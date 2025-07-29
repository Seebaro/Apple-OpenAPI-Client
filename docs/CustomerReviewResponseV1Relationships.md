# CustomerReviewResponseV1Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**review** | [**CustomerReviewResponseV1RelationshipsReview**](CustomerReviewResponseV1RelationshipsReview.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_response_v1_relationships import CustomerReviewResponseV1Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseV1Relationships from a JSON string
customer_review_response_v1_relationships_instance = CustomerReviewResponseV1Relationships.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseV1Relationships.to_json())

# convert the object into a dict
customer_review_response_v1_relationships_dict = customer_review_response_v1_relationships_instance.to_dict()
# create an instance of CustomerReviewResponseV1Relationships from a dict
customer_review_response_v1_relationships_from_dict = CustomerReviewResponseV1Relationships.from_dict(customer_review_response_v1_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


