# Coding-Preparation
For Rest Callout"

Http http = new Http();
HttpRequest newRequest = new HttpRequest();
newRequest.setEndpoint("https://abc.com/animals");
newRequest.setMethod('POST');
newRequest.setHeader('Content-Type', 'application/json;charset= UTF-8');
newRequest.setBody('{"name": "mightyMoose"}');
HttpResponse res = http.send(newRequest);

