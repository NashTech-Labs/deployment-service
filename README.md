## How to make a deployment for an application in kubernetes

For deploying an application in kubernetes, we need a deployment file for the same. 
We have to give name to the deployment `<desired-service-name>`. Then we have to mention the namespace `<namespace>`. Then in selectors, we can give the same name in `<application-name>`. Then we have to give the `<container-name>`, `<image-ref>` for the reference of the image from docker hub, harbor or from local. Then we have introduce env's if there are any. And then in the last, `<port>` is being given the port number of the application.


## Running the template
Just run `kubctl apply -f deployment.yml -n <namespace>`