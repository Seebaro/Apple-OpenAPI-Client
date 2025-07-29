# CustomerReviewResponseLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomerReviewRelationshipsResponseData**](CustomerReviewRelationshipsResponseData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.customer_review_response_linkage_response import CustomerReviewResponseLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerReviewResponseLinkageResponse from a JSON string
customer_review_response_linkage_response_instance = CustomerReviewResponseLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(CustomerReviewResponseLinkageResponse.to_json())

# convert the object into a dict
customer_review_response_linkage_response_dict = customer_review_response_linkage_response_instance.to_dict()
# create an instance of CustomerReviewResponseLinkageResponse from a dict
customer_review_response_linkage_response_from_dict = CustomerReviewResponseLinkageResponse.from_dict(customer_review_response_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


