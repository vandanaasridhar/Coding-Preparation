public class HttpRestCallout {
    
    public static void getUsersFromExternalSystem(){
        
        http httpObj = new Http();
        
        HttpRequest req = new HttpRequest();
        req.setEndpoint('https://reqres.in/api/Users');
        req.setHeader('Content-Type','application/json' );
        req.setMethod('GET');
   
        HttpResponse response = httpObj.send(req);
        system.debug(response.getBody());
        
    }

}
