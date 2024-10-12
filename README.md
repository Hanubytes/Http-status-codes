# Http-status-codes

1xx: Informational
These codes indicate that the request was received and the process is continuing.

100 Continue: The server has received the request headers, and the client should proceed to send the request body.
101 Switching Protocols: The requester has asked the server to switch protocols, and the server has agreed to do so.
102 Processing: The server has received and is processing the request, but no response is available yet (WebDAV).
103 Early Hints: Provides some information about the server's response headers before the final HTTP message is sent.
2xx: Success
These codes indicate that the request was successfully received, understood, and accepted.

200 OK: The request has succeeded.
201 Created: The request has been fulfilled, resulting in the creation of a new resource.
202 Accepted: The request has been accepted for processing, but the processing is not yet complete.
203 Non-Authoritative Information: The server is returning information from another source.
204 No Content: The server successfully processed the request, but is not returning any content.
205 Reset Content: The server processed the request, but the client should reset the view (e.g., clear form data).
206 Partial Content: The server is delivering only part of the resource due to a range header sent by the client.
207 Multi-Status: The message body contains multiple status codes (WebDAV).
208 Already Reported: The members of a DAV binding have already been enumerated in a previous reply (WebDAV).
226 IM Used: The server has fulfilled a request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.
3xx: Redirection
These codes indicate that further action needs to be taken in order to complete the request.

300 Multiple Choices: There are multiple options for the resource the client may follow.
301 Moved Permanently: The resource has been permanently moved to a new URL.
302 Found: The resource has been temporarily moved to a different URL.
303 See Other: The server suggests that the client retrieves the resource from another URI.
304 Not Modified: The resource has not been modified since the last request.
305 Use Proxy: The requested resource is available only through a proxy (deprecated).
307 Temporary Redirect: The request should be repeated with another URI, but future requests should use the original URI.
308 Permanent Redirect: The resource has been permanently moved, and all future requests should be sent to the new URI.
4xx: Client Errors
These codes indicate that there was an error with the request from the client side.

400 Bad Request: The server cannot or will not process the request due to a client error (e.g., malformed request syntax).
401 Unauthorized: Authentication is required and has failed or has not yet been provided.
402 Payment Required: Reserved for future use, often used for digital payment systems.
403 Forbidden: The client does not have permission to access the requested resource.
404 Not Found: The server cannot find the requested resource.
405 Method Not Allowed: The request method is known by the server but has been disabled and cannot be used.
406 Not Acceptable: The requested resource is capable of generating only content not acceptable according to the Accept headers.
407 Proxy Authentication Required: The client must first authenticate itself with the proxy.
408 Request Timeout: The server timed out waiting for the request.
409 Conflict: The request could not be processed because of conflict in the request, such as an edit conflict.
410 Gone: The resource requested is no longer available and will not be available again.
411 Length Required: The request did not specify the length of its content, which is required by the requested resource.
412 Precondition Failed: One or more conditions given in the request header fields evaluated to false.
413 Payload Too Large: The request is larger than the server is willing or able to process.
414 URI Too Long: The URI provided was too long for the server to process.
415 Unsupported Media Type: The request entity has a media type which the server or resource does not support.
416 Range Not Satisfiable: The client has asked for a portion of the file, but the server cannot supply that portion.
417 Expectation Failed: The server cannot meet the requirements of the Expect request-header field.
418 I'm a teapot: Defined in RFC 2324, "Hyper Text Coffee Pot Control Protocol" as an April Fools' joke.
421 Misdirected Request: The request was directed at a server that is unable to produce a response.
422 Unprocessable Entity: The request was well-formed but was unable to be followed due to semantic errors (WebDAV).
423 Locked: The resource being accessed is locked (WebDAV).
424 Failed Dependency: The request failed due to the failure of a previous request (WebDAV).
425 Too Early: Indicates that the server is unwilling to process a request that might be replayed.
426 Upgrade Required: The client should switch to a different protocol such as TLS/1.0.
428 Precondition Required: The origin server requires the request to be conditional.
429 Too Many Requests: The user has sent too many requests in a given amount of time.
431 Request Header Fields Too Large: The server is unwilling to process the request because its header fields are too large.
451 Unavailable For Legal Reasons: The server is denying access to the resource as a consequence of a legal demand.
5xx: Server Errors
These codes indicate that the server failed to fulfill a valid request.

500 Internal Server Error: The server encountered an unexpected condition that prevented it from fulfilling the request.
501 Not Implemented: The server either does not recognize the request method or lacks the ability to fulfill the request.
502 Bad Gateway: The server, while acting as a gateway or proxy, received an invalid response from the upstream server.
503 Service Unavailable: The server is not ready to handle the request, often due to being overloaded or down for maintenance.
504 Gateway Timeout: The server was acting as a gateway or proxy and did not receive a timely response from the upstream server.
505 HTTP Version Not Supported: The server does not support the HTTP protocol version used in the request.
506 Variant Also Negotiates: Transparent content negotiation for the request results in a circular reference.
507 Insufficient Storage: The server is unable to store the representation needed to complete the request (WebDAV).
508 Loop Detected: The server detected an infinite loop while processing the request (WebDAV).
510 Not Extended: Further extensions to the request are required for the server to fulfill it.
511 Network Authentication Required: The client needs to authenticate to gain network access.
