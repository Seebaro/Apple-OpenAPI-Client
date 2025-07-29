# AppPricePointsV3Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPricePointV3]**](AppPricePointV3.md) |  | 
**included** | [**List[AppPricePointsV3ResponseIncludedInner]**](AppPricePointsV3ResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_points_v3_response import AppPricePointsV3Response

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointsV3Response from a JSON string
app_price_points_v3_response_instance = AppPricePointsV3Response.from_json(json)
# print the JSON string representation of the object
print(AppPricePointsV3Response.to_json())

# convert the object into a dict
app_price_points_v3_response_dict = app_price_points_v3_response_instance.to_dict()
# create an instance of AppPricePointsV3Response from a dict
app_price_points_v3_response_from_dict = AppPricePointsV3Response.from_dict(app_price_points_v3_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


