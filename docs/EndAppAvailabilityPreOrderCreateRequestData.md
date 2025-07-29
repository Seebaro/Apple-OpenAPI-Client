# EndAppAvailabilityPreOrderCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**EndAppAvailabilityPreOrderCreateRequestDataRelationships**](EndAppAvailabilityPreOrderCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.end_app_availability_pre_order_create_request_data import EndAppAvailabilityPreOrderCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of EndAppAvailabilityPreOrderCreateRequestData from a JSON string
end_app_availability_pre_order_create_request_data_instance = EndAppAvailabilityPreOrderCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(EndAppAvailabilityPreOrderCreateRequestData.to_json())

# convert the object into a dict
end_app_availability_pre_order_create_request_data_dict = end_app_availability_pre_order_create_request_data_instance.to_dict()
# create an instance of EndAppAvailabilityPreOrderCreateRequestData from a dict
end_app_availability_pre_order_create_request_data_from_dict = EndAppAvailabilityPreOrderCreateRequestData.from_dict(end_app_availability_pre_order_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


