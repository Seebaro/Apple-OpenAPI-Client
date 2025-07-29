# CustomerReview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CustomerReviewAttributes**](CustomerReviewAttributes.md) |  | [optional] 
**relationships** | [**CustomerReviewRelationships**](CustomerReviewRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review import CustomerReview

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReview from a JSON string
customer_review_instance = CustomerReview.from_json(json)
# print the JSON string representation of the object
print(CustomerReview.to_json())

# convert the object into a dict
customer_review_dict = customer_review_instance.to_dict()
# create an instance of CustomerReview from a dict
customer_review_from_dict = CustomerReview.from_dict(customer_review_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


