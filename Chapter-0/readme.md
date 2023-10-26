# React assignment

1. ## &nbsp; What is emment?

   Emmet is self plug-ins / extension in text editor which provide common code snippets using abbrevation , we can customize the abbrevation and its code snippets.
   abbrevation --> html:5 will produce basic html version 5 structures

2. ## &nbsp; What is difference between framework and library ?
   
   library is piece of resuable code which doesn't have any convention , pattern ,structure of program that need to follow.

   framework provide fullfledge structure and architecture to perform the task it serve , it has full
   controll over it.

3. ## &nbsp; What is CDN and when to use it ?
 
    CDN is content delivery network which is network of server across different area in such a way that it can delivery static content much faster than usual.

    used when need to delivery static content.

4. ## &nbsp; Why React is know as React ?

    facebook developer while developing js frontend library they think of making it's perform as
    faster and reactive instantly so it's name came from there. 

5. ## &nbsp; What is crossorigin in script tag ?
   
   origin is combination of three things:
      1. protocal (http / https).
      2. domain name or ip address .
      3. port on which program running.

   when two program let's say client (browser / which need data) need to access or communicate with
   server (which sent data to client) are in different origin then browser throw cors error for
   security reason.

   if server configure to permit the origin by permitting all three things are in allowed list:

     1. access-control-allow-origin - if requested origin is in allowed list on server.
     2. access-control-allow-method - if requested method (get / post /put / delete) is in allowed method on server.
     3. access-control-allow-header - if requested header has data that present on allowed list of header key on server

    simple request - [ get ] method , no credentials  , no custom-header , content-type : text/plain ,
    multipart/form-data , application/x-www-form-urlencoded.

    non-simple request - [post , put ,delete] , cookies as credential , custom header , content-type - application /json 

   if request is non simple request the browser itself send preflight request to server prior to 
   client request, check it is permitted or not , if not then throw cors error by browser.

   crossorigin in script attribute make to communicate between different origin in simple request without cors error.

6. ## &nbsp; What is React and React DOM  ?
     
     both are written in javascript.

     react has core react functionality like create react element and same across all platform like web, ios , andriod , vr.

     react dom has dom manipulation functionality , specific to browser only.

7. ## &nbsp; What is different between react.development.js and react.production.js ?
     
     development.js is for developing , debugging code so it bundle , minify , optimize perform is 
     much lesser than runtime production.js, since it is for debugging it give more error details and also not remove dead code but production.js does.

8. ## &nbsp; What is asyc and defer ?
    
    In html document it exceute html code line by line when it encounter script it start to download and 
    exceute at that time itself in normal script.

    if async attribute used in script then script download side by side when html is executing and
    when it counter the script it will execute by bypassing downloading time and only have execution time execute when it encounter, used when script is independent of other script.

    defer attribute makes to download script side by side when html is executing and 
    not execute when it encounter it execute only there is no html code remains to execute , used whrn script is dependent on other script


