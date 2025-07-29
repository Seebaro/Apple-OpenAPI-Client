# CustomerReviewSummarizationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_date** | **datetime** |  | [optional] 
**locale** | **str** |  | [optional] 
**platform** | [**Platform**](Platform.md) |  | [optional] 
**text** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_summarization_attributes import CustomerReviewSummarizationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewSummarizationAttributes from a JSON string
customer_review_summarization_attributes_instance = CustomerReviewSummarizationAttributes.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewSummarizationAttributes.to_json())

# convert the object into a dict
customer_review_summarization_attributes_dict = customer_review_summarization_attributes_instance.to_dict()
# create an instance of CustomerReviewSummarizationAttributes from a dict
customer_review_summarization_attributes_from_dict = CustomerReviewSummarizationAttributes.from_dict(customer_review_summarization_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


