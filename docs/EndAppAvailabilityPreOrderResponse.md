# EndAppAvailabilityPreOrderResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**EndAppAvailabilityPreOrder**](EndAppAvailabilityPreOrder.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.end_app_availability_pre_order_response import EndAppAvailabilityPreOrderResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EndAppAvailabilityPreOrderResponse from a JSON string
end_app_availability_pre_order_response_instance = EndAppAvailabilityPreOrderResponse.from_json(json)
# print the JSON string representation of the object
print(EndAppAvailabilityPreOrderResponse.to_json())

# convert the object into a dict
end_app_availability_pre_order_response_dict = end_app_availability_pre_order_response_instance.to_dict()
# create an instance of EndAppAvailabilityPreOrderResponse from a dict
end_app_availability_pre_order_response_from_dict = EndAppAvailabilityPreOrderResponse.from_dict(end_app_availability_pre_order_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


