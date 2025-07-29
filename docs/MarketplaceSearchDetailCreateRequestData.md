# MarketplaceSearchDetailCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**MarketplaceSearchDetailCreateRequestDataAttributes**](MarketplaceSearchDetailCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.marketplace_search_detail_create_request_data import MarketplaceSearchDetailCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetailCreateRequestData from a JSON string
marketplace_search_detail_create_request_data_instance = MarketplaceSearchDetailCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetailCreateRequestData.to_json())

# convert the object into a dict
marketplace_search_detail_create_request_data_dict = marketplace_search_detail_create_request_data_instance.to_dict()
# create an instance of MarketplaceSearchDetailCreateRequestData from a dict
marketplace_search_detail_create_request_data_from_dict = MarketplaceSearchDetailCreateRequestData.from_dict(marketplace_search_detail_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


