#Errors

Our API returns standard HTTP success or error status codes.  

In general: Codes in the <var>2xx</var> range indicate success. 

Codes in the <var>4xx</var> range indicate an error that failed given the information provided (e.g., a required parameter was omitted). 

Codes in the <var>5xx</var> range indicate an error with Qebot's servers (e.g., server unavailability).

<!--<aside class="notice">
This error section is stored in a separate file in <code>includes/_errors.md</code>. Slate allows you to optionally separate out your docs into many files...just save them to the <code>includes</code> folder and add them to the top of your <code>index.md</code>'s frontmatter. Files are included in the order listed.
</aside>-->

## HTTP Status Codes

Code | Title | Description
---------- | ----- | -----------
200 | OK | The request was successful.
204 | OK | The request was successful with no body content.
400 | Bad Request | The request was invalid or could not be understood by the server.  This commonly occurs with faulty request encoding or empty requests in create actions.
401 | Unauthorized | Your API key is missing or invalid.
403 | Forbidden | The login is attempting to perform an action it does not have privileges to access. Verify your login credentials are for the appropriate account.
404 | Not Found | The specified resource could not be found.
405 | Method Not Allowed | You tried to access a resouce with an invalid method.
412 | Precondition Failed | The request was unsuccessful because a condition was not met. For example, making a purchase on an inactive tool.
422 | Validation  | Could not process a POST, PUT, or PATCH request because the request is invalid. 
500 | Internal Server Error | We had a problem with our server. Try again later.
503 | Service Unavailable | We're temporarily offline for maintenance. Please try again later.