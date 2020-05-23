# Swagger\Client\PosTaggerApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**posTaggerTagAdjectives**](PosTaggerApi.md#posTaggerTagAdjectives) | **POST** /nlp-v2/pos/tag/adjectives | Part-of-speech tag a string, filter to adjectives
[**posTaggerTagAdverbs**](PosTaggerApi.md#posTaggerTagAdverbs) | **POST** /nlp-v2/pos/tag/adverbs | Part-of-speech tag a string, filter to adverbs
[**posTaggerTagNouns**](PosTaggerApi.md#posTaggerTagNouns) | **POST** /nlp-v2/pos/tag/nouns | Part-of-speech tag a string, filter to nouns
[**posTaggerTagPronouns**](PosTaggerApi.md#posTaggerTagPronouns) | **POST** /nlp-v2/pos/tag/pronouns | Part-of-speech tag a string, filter to pronouns
[**posTaggerTagSentence**](PosTaggerApi.md#posTaggerTagSentence) | **POST** /nlp-v2/pos/tag/sentence | Part-of-speech tag a string
[**posTaggerTagVerbs**](PosTaggerApi.md#posTaggerTagVerbs) | **POST** /nlp-v2/pos/tag/verbs | Part-of-speech tag a string, filter to verbs


# **posTaggerTagAdjectives**
> \Swagger\Client\Model\PosResponse posTaggerTagAdjectives($request)

Part-of-speech tag a string, filter to adjectives

Part-of-speech (POS) tag a string, find the adjectives, and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagAdjectives($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagAdjectives: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **posTaggerTagAdverbs**
> \Swagger\Client\Model\PosResponse posTaggerTagAdverbs($request)

Part-of-speech tag a string, filter to adverbs

Part-of-speech (POS) tag a string, find the adverbs, and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagAdverbs($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagAdverbs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **posTaggerTagNouns**
> \Swagger\Client\Model\PosResponse posTaggerTagNouns($request)

Part-of-speech tag a string, filter to nouns

Part-of-speech (POS) tag a string, find the nouns, and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagNouns($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagNouns: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **posTaggerTagPronouns**
> \Swagger\Client\Model\PosResponse posTaggerTagPronouns($request)

Part-of-speech tag a string, filter to pronouns

Part-of-speech (POS) tag a string, find the pronouns, and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagPronouns($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagPronouns: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **posTaggerTagSentence**
> \Swagger\Client\Model\PosResponse posTaggerTagSentence($request)

Part-of-speech tag a string

Part-of-speech (POS) tag a string and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagSentence($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagSentence: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **posTaggerTagVerbs**
> \Swagger\Client\Model\PosResponse posTaggerTagVerbs($request)

Part-of-speech tag a string, filter to verbs

Part-of-speech (POS) tag a string, find the verbs, and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerTagVerbs($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerApi->posTaggerTagVerbs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

