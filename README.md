 # JBPM-RestAPI-
Main Process..

<img width="1785" alt="image" src="https://user-images.githubusercontent.com/67383223/157454548-7a2940da-53b5-4727-a626-b18fdb67ded8.png">
Reusable process Assignments ..
<img width="1763" alt="image" src="https://user-images.githubusercontent.com/67383223/157454732-0bc99d08-45a4-4489-b801-bc7b51b4e364.png">


Sub process..
<img width="1782" alt="image" src="https://user-images.githubusercontent.com/67383223/157455075-cbd2d192-f22b-4626-a60c-80bb7063bc60.png">

Rest Task assignmnets 

<img width="1785" alt="image" src="https://user-images.githubusercontent.com/67383223/157455188-8f458daa-05ce-4283-ae50-59d49e2feb1a.png">

Object class

<img width="1791" alt="image" src="https://user-images.githubusercontent.com/67383223/157455380-cd8d4110-9cb5-4745-b67a-8b4815b48ffb.png">

Build and deploy the process...

Start the process with custom parameters...
<img width="1769" alt="image" src="https://user-images.githubusercontent.com/67383223/157455552-c4c3fdc7-3a7e-45fa-9f03-c0feebdf912a.png">


Process Variables after completed the process ...
![image](https://user-images.githubusercontent.com/67383223/157454180-d59f398b-90a3-4f93-bad1-bf74fd79d308.png)




From the Server logs we can see the success and failure state.

Success Logs ...
19:11:25,911 INFO  [stdout] (default task-64) inside main process===
19:11:25,922 INFO  [stdout] (default task-64) inside sub process
19:11:25,926 INFO  [stdout] (default task-64) inside rest process
19:11:26,932 INFO  [stdout] (default task-64) outside rest process
19:11:26,932 INFO  [stdout] (default task-64) status===200
19:11:26,932 INFO  [stdout] (default task-64) Response==={"status":"success","data":{"id":2889},"message":"Successfully! Record has been added."}
19:11:26,942 INFO  [stdout] (default task-64) status===200
19:11:26,945 INFO  [stdout] (default task-64) Record updated successfully ===

![image](https://user-images.githubusercontent.com/67383223/157454012-a4c672a1-50fc-41ea-affd-c9b60768486b.png)

Failure logs ....

19:10:59,087 INFO  [stdout] (default task-64) inside main process===
19:10:59,097 INFO  [stdout] (default task-64) inside sub process
19:10:59,098 INFO  [stdout] (default task-64) inside rest process
19:11:01,265 WARN  [org.jbpm.process.workitem.rest.RESTWorkItemHandler] (default task-64) Unsuccessful response from REST server (status: 429, endpoint: http://dummy.restapiexample.com/api/v1/create, response: {
    "message": "Too Many Attempts."
}
19:11:01,268 INFO  [stdout] (default task-64) outside rest process
19:11:01,269 INFO  [stdout] (default task-64) status===429
19:11:01,269 INFO  [stdout] (default task-64) Response===null
19:11:01,279 INFO  [stdout] (default task-64) status===429
19:11:01,282 INFO  [stdout] (default task-64) Record update failed===

![image](https://user-images.githubusercontent.com/67383223/157453900-366eee42-0826-47bb-94b6-d511b2e0a485.png)
