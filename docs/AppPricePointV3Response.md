# AppPricePointV3Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppPricePointV3**](AppPricePointV3.md) |  | 
**included** | [**List[AppPricePointsV3ResponseIncludedInner]**](AppPricePointsV3ResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_price_point_v3_response import AppPricePointV3Response

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointV3Response from a JSON string
app_price_point_v3_response_instance = AppPricePointV3Response.from_json(json)
# print the JSON string representation of the object
print(AppPricePointV3Response.to_json())

# convert the object into a dict
app_price_point_v3_response_dict = app_price_point_v3_response_instance.to_dict()
# create an instance of AppPricePointV3Response from a dict
app_price_point_v3_response_from_dict = AppPricePointV3Response.from_dict(app_price_point_v3_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


