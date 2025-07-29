# MarketplaceSearchDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**MarketplaceSearchDetailAttributes**](MarketplaceSearchDetailAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_search_detail import MarketplaceSearchDetail

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetail from a JSON string
marketplace_search_detail_instance = MarketplaceSearchDetail.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetail.to_json())

# convert the object into a dict
marketplace_search_detail_dict = marketplace_search_detail_instance.to_dict()
# create an instance of MarketplaceSearchDetail from a dict
marketplace_search_detail_from_dict = MarketplaceSearchDetail.from_dict(marketplace_search_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


