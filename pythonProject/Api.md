# activity.Api

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activities_pass_activities_get**](Api.md#activities_pass_activities_get) | **GET** /activities/{pass-activities} | 获取所有活动
[**activity_acti_name_get**](Api.md#activity_acti_name_get) | **GET** /activity/{acti_name} | 获取活动信息
[**activity_comment_delete**](Api.md#activity_comment_delete) | **DELETE** /activity-comment | 删除活动评论
[**activity_comment_post**](Api.md#activity_comment_post) | **POST** /activity-comment | 发表活动评论
[**activity_emergency_post**](Api.md#activity_emergency_post) | **POST** /activity/emergency | 上传紧急预案
[**activity_information_post**](Api.md#activity_information_post) | **POST** /activity/information | 填写活动信息
[**activity_like_delete**](Api.md#activity_like_delete) | **DELETE** /activity-like | 取消活动点赞
[**activity_like_post**](Api.md#activity_like_post) | **POST** /activity-like | 活动点赞
[**activity_planning_post**](Api.md#activity_planning_post) | **POST** /activity/planning | 上传策划案
[**activity_post**](Api.md#activity_post) | **POST** /activity | 发布活动
[**activity_poster_post**](Api.md#activity_poster_post) | **POST** /activity/poster | 上传海报
[**dynamic_comment_delete**](Api.md#dynamic_comment_delete) | **DELETE** /dynamic-comment | 删除动态评论
[**dynamic_comment_get**](Api.md#dynamic_comment_get) | **GET** /dynamic/{comment} | 获取动态评论
[**dynamic_comment_post**](Api.md#dynamic_comment_post) | **POST** /dynamic-comment | 发表动态评论
[**dynamic_delete**](Api.md#dynamic_delete) | **DELETE** /dynamic | 删除动态
[**dynamic_dynamic_get**](Api.md#dynamic_dynamic_get) | **GET** /dynamic/{dynamic} | 获取动态信息
[**dynamic_like_delete**](Api.md#dynamic_like_delete) | **DELETE** /dynamic-like | 取消动态点赞
[**dynamic_like_post**](Api.md#dynamic_like_post) | **POST** /dynamic-like | 动态点赞
[**dynamic_post**](Api.md#dynamic_post) | **POST** /dynamic | 发布动态
[**dynamics_dynamics_get**](Api.md#dynamics_dynamics_get) | **GET** /dynamics/{dynamics} | 获取所有动态
[**follow_delete**](Api.md#follow_delete) | **DELETE** /follow | 取消关注
[**follow_post**](Api.md#follow_post) | **POST** /follow | 添加关注
[**login_app_post**](Api.md#login_app_post) | **POST** /login/app | 小程序登录【微信】
[**refresh_post**](Api.md#refresh_post) | **POST** /refresh | 刷新token【微信】
[**user_add_administrator_post**](Api.md#user_add_administrator_post) | **POST** /user/add_administrator | 添加管理员
[**user_del_administrator_delete**](Api.md#user_del_administrator_delete) | **DELETE** /user/del_administrator | 删除管理员
[**user_id_get**](Api.md#user_id_get) | **GET** /user/{id} | 获取用户信息
[**users_users_get**](Api.md#users_users_get) | **GET** /users/{users} | 获取所有用户


# **activities_pass_activities_get**
> InlineResponse2006 activities_pass_activities_get(pass_activities)

获取所有活动

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    pass_activities = 'pass_activities_example' # str | 

    try:
        # 获取所有活动
        api_response = api_instance.activities_pass_activities_get(pass_activities)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activities_pass_activities_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_activities** | **str**|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_acti_name_get**
> InlineResponse2007 activity_acti_name_get(acti_name)

获取活动信息

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    acti_name = 'acti_name_example' # str | 

    try:
        # 获取活动信息
        api_response = api_instance.activity_acti_name_get(acti_name)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_acti_name_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acti_name** | **str**|  | 

### Return type

[**InlineResponse2007**](InlineResponse2007.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 记录不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_comment_delete**
> object activity_comment_delete()

删除活动评论

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 删除活动评论
        api_response = api_instance.activity_comment_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_comment_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_comment_post**
> object activity_comment_post()

发表活动评论

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 发表活动评论
        api_response = api_instance.activity_comment_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_comment_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_emergency_post**
> InlineResponse2002 activity_emergency_post(emergency=emergency)

上传紧急预案

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    emergency = '/path/to/file' # file |  (optional)

    try:
        # 上传紧急预案
        api_response = api_instance.activity_emergency_post(emergency=emergency)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_emergency_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emergency** | **file**|  | [optional] 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_information_post**
> InlineResponse2004 activity_information_post(acti_name, location, begin_time, brief)

填写活动信息

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    acti_name = 'acti_name_example' # str | 
location = 'location_example' # str | 
begin_time = 'begin_time_example' # str | 
brief = 'brief_example' # str | 

    try:
        # 填写活动信息
        api_response = api_instance.activity_information_post(acti_name, location, begin_time, brief)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_information_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acti_name** | **str**|  | 
 **location** | **str**|  | 
 **begin_time** | **str**|  | 
 **brief** | **str**|  | 

### Return type

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**400** | 信息不完整 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_like_delete**
> object activity_like_delete()

取消活动点赞

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 取消活动点赞
        api_response = api_instance.activity_like_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_like_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_like_post**
> object activity_like_post()

活动点赞

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 活动点赞
        api_response = api_instance.activity_like_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_like_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_planning_post**
> InlineResponse2002 activity_planning_post(planning=planning)

上传策划案

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    planning = '/path/to/file' # file |  (optional)

    try:
        # 上传策划案
        api_response = api_instance.activity_planning_post(planning=planning)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_planning_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **planning** | **file**|  | [optional] 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_post**
> InlineResponse404 activity_post()

发布活动

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 发布活动
        api_response = api_instance.activity_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse404**](InlineResponse404.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**400** | 信息不完整 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **activity_poster_post**
> InlineResponse2001 activity_poster_post(poster)

上传海报

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    poster = '/path/to/file' # file | 

    try:
        # 上传海报
        api_response = api_instance.activity_poster_post(poster)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->activity_poster_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **poster** | **file**|  | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_comment_delete**
> object dynamic_comment_delete()

删除动态评论

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 删除动态评论
        api_response = api_instance.dynamic_comment_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_comment_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_comment_get**
> InlineResponse2006 dynamic_comment_get(comment)

获取动态评论

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    comment = 'comment_example' # str | 

    try:
        # 获取动态评论
        api_response = api_instance.dynamic_comment_get(comment)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_comment_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **comment** | **str**|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 记录不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_comment_post**
> object dynamic_comment_post()

发表动态评论

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 发表动态评论
        api_response = api_instance.dynamic_comment_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_comment_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_delete**
> object dynamic_delete()

删除动态

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 删除动态
        api_response = api_instance.dynamic_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_dynamic_get**
> InlineResponse2008 dynamic_dynamic_get(dynamic)

获取动态信息

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    dynamic = 'dynamic_example' # str | 

    try:
        # 获取动态信息
        api_response = api_instance.dynamic_dynamic_get(dynamic)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_dynamic_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dynamic** | **str**|  | 

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 记录不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_like_delete**
> object dynamic_like_delete()

取消动态点赞

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 取消动态点赞
        api_response = api_instance.dynamic_like_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_like_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_like_post**
> object dynamic_like_post()

动态点赞

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 动态点赞
        api_response = api_instance.dynamic_like_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_like_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamic_post**
> InlineResponse2005 dynamic_post(dynamic=dynamic)

发布动态

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    dynamic = 'dynamic_example' # str |  (optional)

    try:
        # 发布动态
        api_response = api_instance.dynamic_post(dynamic=dynamic)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamic_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dynamic** | **str**|  | [optional] 

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dynamics_dynamics_get**
> InlineResponse2006 dynamics_dynamics_get(dynamics)

获取所有动态

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    dynamics = 'dynamics_example' # str | 

    try:
        # 获取所有动态
        api_response = api_instance.dynamics_dynamics_get(dynamics)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->dynamics_dynamics_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dynamics** | **str**|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **follow_delete**
> object follow_delete()

取消关注

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 取消关注
        api_response = api_instance.follow_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->follow_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **follow_post**
> object follow_post()

添加关注

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 添加关注
        api_response = api_instance.follow_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->follow_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login_app_post**
> object login_app_post(access_token, openid=openid)

小程序登录【微信】

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    access_token = 'access_token_example' # str | 
openid = 'openid_example' # str |  (optional)

    try:
        # 小程序登录【微信】
        api_response = api_instance.login_app_post(access_token, openid=openid)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->login_app_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **access_token** | **str**|  | 
 **openid** | **str**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refresh_post**
> object refresh_post()

刷新token【微信】

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 刷新token【微信】
        api_response = api_instance.refresh_post()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->refresh_post: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_add_administrator_post**
> InlineResponse2003 user_add_administrator_post(body=body)

添加管理员

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    body = 464646545132 # str |  (optional)

    try:
        # 添加管理员
        api_response = api_instance.user_add_administrator_post(body=body)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->user_add_administrator_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **str**|  | [optional] 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: text/plain
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 用户不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_del_administrator_delete**
> InlineResponse404 user_del_administrator_delete()

删除管理员

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    
    try:
        # 删除管理员
        api_response = api_instance.user_del_administrator_delete()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->user_del_administrator_delete: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse404**](InlineResponse404.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 记录不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_id_get**
> InlineResponse200 user_id_get(id)

获取用户信息

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    id = 'id_example' # str | 

    try:
        # 获取用户信息
        api_response = api_instance.user_id_get(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->user_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 用户不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **users_users_get**
> InlineResponse2006 users_users_get(users)

获取所有用户

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.Api(api_client)
    users = 'users_example' # str | 

    try:
        # 获取所有用户
        api_response = api_instance.users_users_get(users)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling Api->users_users_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **users** | **str**|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

