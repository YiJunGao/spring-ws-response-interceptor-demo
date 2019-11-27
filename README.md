# spring-ws-response-interceptor-demo

Configure Interceptor using Spring Java Configuration
Now we have written our CustomEndpointInterceptor we need to tell Spring WS to use it. We do this by overriding the addInterceptors method of the WsConfigurerAdapter. We define a global interceptor by just adding it to the interceptors list. For an endpoint specific interceptor we must use the PayloadRootSmartSoapEndpointInterceptor class which takes a delegate interceptor, a namespace and a localPart as arguments. The interceptor uses the namespace and local part to map the interceptor to the endpoint.

from:https://memorynotfound.com/spring-ws-intercept-request-response-soap-messages/
