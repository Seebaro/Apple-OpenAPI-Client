# CustomerReviewSummarization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CustomerReviewSummarizationAttributes**](CustomerReviewSummarizationAttributes.md) |  | [optional] 
**relationships** | [**CustomerReviewSummarizationRelationships**](CustomerReviewSummarizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.customer_review_summarization import CustomerReviewSummarization

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewSummarization from a JSON string
customer_review_summarization_instance = CustomerReviewSummarization.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewSummarization.to_json())

# convert the object into a dict
customer_review_summarization_dict = customer_review_summarization_instance.to_dict()
# create an instance of CustomerReviewSummarization from a dict
customer_review_summarization_from_dict = CustomerReviewSummarization.from_dict(customer_review_summarization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


