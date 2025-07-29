# AppPricePointV3EqualizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPriceV2RelationshipsAppPricePointData]**](AppPriceV2RelationshipsAppPricePointData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_point_v3_equalizations_linkages_response import AppPricePointV3EqualizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointV3EqualizationsLinkagesResponse from a JSON string
app_price_point_v3_equalizations_linkages_response_instance = AppPricePointV3EqualizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPricePointV3EqualizationsLinkagesResponse.to_json())

# convert the object into a dict
app_price_point_v3_equalizations_linkages_response_dict = app_price_point_v3_equalizations_linkages_response_instance.to_dict()
# create an instance of AppPricePointV3EqualizationsLinkagesResponse from a dict
app_price_point_v3_equalizations_linkages_response_from_dict = AppPricePointV3EqualizationsLinkagesResponse.from_dict(app_price_point_v3_equalizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


