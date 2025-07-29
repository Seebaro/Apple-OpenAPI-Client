# openapi_client.SubscriptionGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_groups_create_instance**](SubscriptionGroupsApi.md#subscription_groups_create_instance) | **POST** /v1/subscriptionGroups | 
[**subscription_groups_delete_instance**](SubscriptionGroupsApi.md#subscription_groups_delete_instance) | **DELETE** /v1/subscriptionGroups/{id} | 
[**subscription_groups_get_instance**](SubscriptionGroupsApi.md#subscription_groups_get_instance) | **GET** /v1/subscriptionGroups/{id} | 
[**subscription_groups_subscription_group_localizations_get_to_many_related**](SubscriptionGroupsApi.md#subscription_groups_subscription_group_localizations_get_to_many_related) | **GET** /v1/subscriptionGroups/{id}/subscriptionGroupLocalizations | 
[**subscription_groups_subscription_group_localizations_get_to_many_relationship**](SubscriptionGroupsApi.md#subscription_groups_subscription_group_localizations_get_to_many_relationship) | **GET** /v1/subscriptionGroups/{id}/relationships/subscriptionGroupLocalizations | 
[**subscription_groups_subscriptions_get_to_many_related**](SubscriptionGroupsApi.md#subscription_groups_subscriptions_get_to_many_related) | **GET** /v1/subscriptionGroups/{id}/subscriptions | 
[**subscription_groups_subscriptions_get_to_many_relationship**](SubscriptionGroupsApi.md#subscription_groups_subscriptions_get_to_many_relationship) | **GET** /v1/subscriptionGroups/{id}/relationships/subscriptions | 
[**subscription_groups_update_instance**](SubscriptionGroupsApi.md#subscription_groups_update_instance) | **PATCH** /v1/subscriptionGroups/{id} | 


# **subscription_groups_create_instance**
> SubscriptionGroupResponse subscription_groups_create_instance(subscription_group_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_create_request import SubscriptionGroupCreateRequest
from openapi_client.models.subscription_group_response import SubscriptionGroupResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    subscription_group_create_request = openapi_client.SubscriptionGroupCreateRequest() # SubscriptionGroupCreateRequest | SubscriptionGroup representation

    try:
        api_response = api_instance.subscription_groups_create_instance(subscription_group_create_request)
        print("The response of SubscriptionGroupsApi->subscription_groups_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_group_create_request** | [**SubscriptionGroupCreateRequest**](SubscriptionGroupCreateRequest.md)| SubscriptionGroup representation | 

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**201** | Single SubscriptionGroup |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_delete_instance**
> subscription_groups_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.subscription_groups_delete_instance(id)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_get_instance**
> SubscriptionGroupResponse subscription_groups_get_instance(id, fields_subscription_groups=fields_subscription_groups, fields_subscriptions=fields_subscriptions, fields_subscription_group_localizations=fields_subscription_group_localizations, include=include, limit_subscription_group_localizations=limit_subscription_group_localizations, limit_subscriptions=limit_subscriptions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_response import SubscriptionGroupResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_groups = ['fields_subscription_groups_example'] # List[str] | the fields to include for returned resources of type subscriptionGroups (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_subscription_group_localizations = ['fields_subscription_group_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionGroupLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subscription_group_localizations = 56 # int | maximum number of related subscriptionGroupLocalizations returned (when they are included) (optional)
    limit_subscriptions = 56 # int | maximum number of related subscriptions returned (when they are included) (optional)

    try:
        api_response = api_instance.subscription_groups_get_instance(id, fields_subscription_groups=fields_subscription_groups, fields_subscriptions=fields_subscriptions, fields_subscription_group_localizations=fields_subscription_group_localizations, include=include, limit_subscription_group_localizations=limit_subscription_group_localizations, limit_subscriptions=limit_subscriptions)
        print("The response of SubscriptionGroupsApi->subscription_groups_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroups | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_subscription_group_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroupLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_subscription_group_localizations** | **int**| maximum number of related subscriptionGroupLocalizations returned (when they are included) | [optional] 
 **limit_subscriptions** | **int**| maximum number of related subscriptions returned (when they are included) | [optional] 

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single SubscriptionGroup |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_subscription_group_localizations_get_to_many_related**
> SubscriptionGroupLocalizationsResponse subscription_groups_subscription_group_localizations_get_to_many_related(id, fields_subscription_group_localizations=fields_subscription_group_localizations, fields_subscription_groups=fields_subscription_groups, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_localizations_response import SubscriptionGroupLocalizationsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_group_localizations = ['fields_subscription_group_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionGroupLocalizations (optional)
    fields_subscription_groups = ['fields_subscription_groups_example'] # List[str] | the fields to include for returned resources of type subscriptionGroups (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_groups_subscription_group_localizations_get_to_many_related(id, fields_subscription_group_localizations=fields_subscription_group_localizations, fields_subscription_groups=fields_subscription_groups, limit=limit, include=include)
        print("The response of SubscriptionGroupsApi->subscription_groups_subscription_group_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_subscription_group_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_group_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroupLocalizations | [optional] 
 **fields_subscription_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroups | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionGroupLocalizationsResponse**](SubscriptionGroupLocalizationsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionGroupLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_subscription_group_localizations_get_to_many_relationship**
> SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse subscription_groups_subscription_group_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_subscription_group_localizations_linkages_response import SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_groups_subscription_group_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionGroupsApi->subscription_groups_subscription_group_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_subscription_group_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse**](SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_subscriptions_get_to_many_related**
> SubscriptionsResponse subscription_groups_subscriptions_get_to_many_related(id, filter_product_id=filter_product_id, filter_name=filter_name, filter_state=filter_state, sort=sort, fields_subscriptions=fields_subscriptions, fields_subscription_localizations=fields_subscription_localizations, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscription_groups=fields_subscription_groups, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_prices=fields_subscription_prices, fields_promoted_purchases=fields_promoted_purchases, fields_subscription_availabilities=fields_subscription_availabilities, fields_win_back_offers=fields_win_back_offers, fields_subscription_images=fields_subscription_images, limit=limit, include=include, limit_subscription_localizations=limit_subscription_localizations, limit_introductory_offers=limit_introductory_offers, limit_promotional_offers=limit_promotional_offers, limit_offer_codes=limit_offer_codes, limit_prices=limit_prices, limit_win_back_offers=limit_win_back_offers, limit_images=limit_images)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscriptions_response import SubscriptionsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_product_id = ['filter_product_id_example'] # List[str] | filter by attribute 'productId' (optional)
    filter_name = ['filter_name_example'] # List[str] | filter by attribute 'name' (optional)
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_subscription_localizations = ['fields_subscription_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionLocalizations (optional)
    fields_subscription_app_store_review_screenshots = ['fields_subscription_app_store_review_screenshots_example'] # List[str] | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots (optional)
    fields_subscription_groups = ['fields_subscription_groups_example'] # List[str] | the fields to include for returned resources of type subscriptionGroups (optional)
    fields_subscription_introductory_offers = ['fields_subscription_introductory_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionIntroductoryOffers (optional)
    fields_subscription_promotional_offers = ['fields_subscription_promotional_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionPromotionalOffers (optional)
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    fields_subscription_prices = ['fields_subscription_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionPrices (optional)
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_subscription_availabilities = ['fields_subscription_availabilities_example'] # List[str] | the fields to include for returned resources of type subscriptionAvailabilities (optional)
    fields_win_back_offers = ['fields_win_back_offers_example'] # List[str] | the fields to include for returned resources of type winBackOffers (optional)
    fields_subscription_images = ['fields_subscription_images_example'] # List[str] | the fields to include for returned resources of type subscriptionImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subscription_localizations = 56 # int | maximum number of related subscriptionLocalizations returned (when they are included) (optional)
    limit_introductory_offers = 56 # int | maximum number of related introductoryOffers returned (when they are included) (optional)
    limit_promotional_offers = 56 # int | maximum number of related promotionalOffers returned (when they are included) (optional)
    limit_offer_codes = 56 # int | maximum number of related offerCodes returned (when they are included) (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)
    limit_win_back_offers = 56 # int | maximum number of related winBackOffers returned (when they are included) (optional)
    limit_images = 56 # int | maximum number of related images returned (when they are included) (optional)

    try:
        api_response = api_instance.subscription_groups_subscriptions_get_to_many_related(id, filter_product_id=filter_product_id, filter_name=filter_name, filter_state=filter_state, sort=sort, fields_subscriptions=fields_subscriptions, fields_subscription_localizations=fields_subscription_localizations, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscription_groups=fields_subscription_groups, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_prices=fields_subscription_prices, fields_promoted_purchases=fields_promoted_purchases, fields_subscription_availabilities=fields_subscription_availabilities, fields_win_back_offers=fields_win_back_offers, fields_subscription_images=fields_subscription_images, limit=limit, include=include, limit_subscription_localizations=limit_subscription_localizations, limit_introductory_offers=limit_introductory_offers, limit_promotional_offers=limit_promotional_offers, limit_offer_codes=limit_offer_codes, limit_prices=limit_prices, limit_win_back_offers=limit_win_back_offers, limit_images=limit_images)
        print("The response of SubscriptionGroupsApi->subscription_groups_subscriptions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_subscriptions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_product_id** | [**List[str]**](str.md)| filter by attribute &#39;productId&#39; | [optional] 
 **filter_name** | [**List[str]**](str.md)| filter by attribute &#39;name&#39; | [optional] 
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_subscription_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionLocalizations | [optional] 
 **fields_subscription_app_store_review_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional] 
 **fields_subscription_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroups | [optional] 
 **fields_subscription_introductory_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional] 
 **fields_subscription_promotional_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPromotionalOffers | [optional] 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **fields_subscription_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPrices | [optional] 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_subscription_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAvailabilities | [optional] 
 **fields_win_back_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOffers | [optional] 
 **fields_subscription_images** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_subscription_localizations** | **int**| maximum number of related subscriptionLocalizations returned (when they are included) | [optional] 
 **limit_introductory_offers** | **int**| maximum number of related introductoryOffers returned (when they are included) | [optional] 
 **limit_promotional_offers** | **int**| maximum number of related promotionalOffers returned (when they are included) | [optional] 
 **limit_offer_codes** | **int**| maximum number of related offerCodes returned (when they are included) | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 
 **limit_win_back_offers** | **int**| maximum number of related winBackOffers returned (when they are included) | [optional] 
 **limit_images** | **int**| maximum number of related images returned (when they are included) | [optional] 

### Return type

[**SubscriptionsResponse**](SubscriptionsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of Subscriptions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_subscriptions_get_to_many_relationship**
> SubscriptionGroupSubscriptionsLinkagesResponse subscription_groups_subscriptions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_subscriptions_linkages_response import SubscriptionGroupSubscriptionsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_groups_subscriptions_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionGroupsApi->subscription_groups_subscriptions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_subscriptions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionGroupSubscriptionsLinkagesResponse**](SubscriptionGroupSubscriptionsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_groups_update_instance**
> SubscriptionGroupResponse subscription_groups_update_instance(id, subscription_group_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_response import SubscriptionGroupResponse
from openapi_client.models.subscription_group_update_request import SubscriptionGroupUpdateRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_group_update_request = openapi_client.SubscriptionGroupUpdateRequest() # SubscriptionGroupUpdateRequest | SubscriptionGroup representation

    try:
        api_response = api_instance.subscription_groups_update_instance(id, subscription_group_update_request)
        print("The response of SubscriptionGroupsApi->subscription_groups_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupsApi->subscription_groups_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_group_update_request** | [**SubscriptionGroupUpdateRequest**](SubscriptionGroupUpdateRequest.md)| SubscriptionGroup representation | 

### Return type

[**SubscriptionGroupResponse**](SubscriptionGroupResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**200** | Single SubscriptionGroup |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

