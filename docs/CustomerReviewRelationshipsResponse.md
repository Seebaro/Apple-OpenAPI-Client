# CustomerReviewRelationshipsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**CustomerReviewRelationshipsResponseData**](CustomerReviewRelationshipsResponseData.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_relationships_response import CustomerReviewRelationshipsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewRelationshipsResponse from a JSON string
customer_review_relationships_response_instance = CustomerReviewRelationshipsResponse.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewRelationshipsResponse.to_json())

# convert the object into a dict
customer_review_relationships_response_dict = customer_review_relationships_response_instance.to_dict()
# create an instance of CustomerReviewRelationshipsResponse from a dict
customer_review_relationships_response_from_dict = CustomerReviewRelationshipsResponse.from_dict(customer_review_relationships_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


