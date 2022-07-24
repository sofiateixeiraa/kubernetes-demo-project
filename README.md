# ☸️ Kubernetes Demo Project

Objective: Mongo express when accessed through a browser requests the mongoDB pod (eg: create a new database via web browser)

It was created a MongoDB pod with an internal service (no external requests are allowed to the pod).
A Mongo Express deployment that contains the info needed to access the DB through Env variables.
MongoDB URL are needed and a DB Username and Password so it was created a Configmap with the DB Url and a Secret with DB Username and Password. Both were referenced in the deployment file of Mongo Express.
Mongo Express needs to be accessed through a web browser so an external service was created too.

![final step](/last-step.png)
