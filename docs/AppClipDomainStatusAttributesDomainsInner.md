# AppClipDomainStatusAttributesDomainsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** |  | [optional] 
**is_valid** | **bool** |  | [optional] 
**last_updated_date** | **datetime** |  | [optional] 
**error_code** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_domain_status_attributes_domains_inner import AppClipDomainStatusAttributesDomainsInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDomainStatusAttributesDomainsInner from a JSON string
app_clip_domain_status_attributes_domains_inner_instance = AppClipDomainStatusAttributesDomainsInner.from_json(json)
# print the JSON string representation of the object
print(AppClipDomainStatusAttributesDomainsInner.to_json())

# convert the object into a dict
app_clip_domain_status_attributes_domains_inner_dict = app_clip_domain_status_attributes_domains_inner_instance.to_dict()
# create an instance of AppClipDomainStatusAttributesDomainsInner from a dict
app_clip_domain_status_attributes_domains_inner_from_dict = AppClipDomainStatusAttributesDomainsInner.from_dict(app_clip_domain_status_attributes_domains_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


