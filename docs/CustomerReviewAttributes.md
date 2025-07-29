# CustomerReviewAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rating** | **int** |  | [optional] 
**title** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**reviewer_nickname** | **str** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**territory** | [**TerritoryCode**](TerritoryCode.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_attributes import CustomerReviewAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewAttributes from a JSON string
customer_review_attributes_instance = CustomerReviewAttributes.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewAttributes.to_json())

# convert the object into a dict
customer_review_attributes_dict = customer_review_attributes_instance.to_dict()
# create an instance of CustomerReviewAttributes from a dict
customer_review_attributes_from_dict = CustomerReviewAttributes.from_dict(customer_review_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


