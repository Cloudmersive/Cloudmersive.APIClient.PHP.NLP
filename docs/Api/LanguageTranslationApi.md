# Swagger\Client\LanguageTranslationApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**languageTranslationTranslateDeuToEng**](LanguageTranslationApi.md#languageTranslationTranslateDeuToEng) | **POST** /nlp-v2/translate/language/deu/to/eng | Translate German to English text with Deep Learning AI
[**languageTranslationTranslateEngToDeu**](LanguageTranslationApi.md#languageTranslationTranslateEngToDeu) | **POST** /nlp-v2/translate/language/eng/to/deu | Translate English to German text with Deep Learning AI
[**languageTranslationTranslateEngToFra**](LanguageTranslationApi.md#languageTranslationTranslateEngToFra) | **POST** /nlp-v2/translate/language/eng/to/fra | Translate English to French text with Deep Learning AI
[**languageTranslationTranslateEngToRus**](LanguageTranslationApi.md#languageTranslationTranslateEngToRus) | **POST** /nlp-v2/translate/language/eng/to/rus | Translate English to Russian text with Deep Learning AI
[**languageTranslationTranslateFraToEng**](LanguageTranslationApi.md#languageTranslationTranslateFraToEng) | **POST** /nlp-v2/translate/language/fra/to/eng | Translate French to English text with Deep Learning AI
[**languageTranslationTranslateRusToEng**](LanguageTranslationApi.md#languageTranslationTranslateRusToEng) | **POST** /nlp-v2/translate/language/rus/to/eng | Translate Russian to English text with Deep Learning AI


# **languageTranslationTranslateDeuToEng**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateDeuToEng($input)

Translate German to English text with Deep Learning AI

Automatically translates input text in German to output text in English using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateDeuToEng($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateDeuToEng: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **languageTranslationTranslateEngToDeu**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateEngToDeu($input)

Translate English to German text with Deep Learning AI

Automatically translates input text in English to output text in German using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateEngToDeu($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateEngToDeu: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **languageTranslationTranslateEngToFra**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateEngToFra($input)

Translate English to French text with Deep Learning AI

Automatically translates input text in English to output text in French using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateEngToFra($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateEngToFra: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **languageTranslationTranslateEngToRus**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateEngToRus($input)

Translate English to Russian text with Deep Learning AI

Automatically translates input text in English to output text in Russian using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateEngToRus($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateEngToRus: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **languageTranslationTranslateFraToEng**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateFraToEng($input)

Translate French to English text with Deep Learning AI

Automatically translates input text in French to output text in English using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateFraToEng($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateFraToEng: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **languageTranslationTranslateRusToEng**
> \Swagger\Client\Model\LanguageTranslationResponse languageTranslationTranslateRusToEng($input)

Translate Russian to English text with Deep Learning AI

Automatically translates input text in Russian to output text in English using advanced Deep Learning and Neural NLP.  Consumes 1-2 API calls per input sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\LanguageTranslationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\LanguageTranslationRequest(); // \Swagger\Client\Model\LanguageTranslationRequest | Input translation request

try {
    $result = $apiInstance->languageTranslationTranslateRusToEng($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LanguageTranslationApi->languageTranslationTranslateRusToEng: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\LanguageTranslationRequest**](../Model/LanguageTranslationRequest.md)| Input translation request |

### Return type

[**\Swagger\Client\Model\LanguageTranslationResponse**](../Model/LanguageTranslationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

