# AppAppPriceScheduleLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppAppPriceScheduleLinkageResponseData**](AppAppPriceScheduleLinkageResponseData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_app_price_schedule_linkage_response import AppAppPriceScheduleLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppPriceScheduleLinkageResponse from a JSON string
app_app_price_schedule_linkage_response_instance = AppAppPriceScheduleLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppPriceScheduleLinkageResponse.to_json())

# convert the object into a dict
app_app_price_schedule_linkage_response_dict = app_app_price_schedule_linkage_response_instance.to_dict()
# create an instance of AppAppPriceScheduleLinkageResponse from a dict
app_app_price_schedule_linkage_response_from_dict = AppAppPriceScheduleLinkageResponse.from_dict(app_app_price_schedule_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


