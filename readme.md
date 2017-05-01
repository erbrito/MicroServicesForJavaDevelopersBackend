This project is consumed by https://github.com/erbrito/MicroServicesForJavaDevelopersSpringBoot




to launch on OpenShift inside a project, execute:

$ oc new-app --docker-image="erbrito/backend:1.0" --name=backend -e DEPLOY_DIR=/maven
--> Found Docker image e1f46f5 (2 days old) from Docker Hub for "erbrito/backend:1.0"

    * An image stream will be created as "backend:1.0" that will track this image
    * This image will be deployed in deployment config "backend"
    * Ports 8080/tcp, 8778/tcp, 9779/tcp will be load balanced by service "backend"
      * Other containers can access this service through the hostname "backend"

--> Creating resources ...
    imagestream "backend" created
    deploymentconfig "backend" created
    service "backend" created
--> Success
    Run 'oc status' to view your app.