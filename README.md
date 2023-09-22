## Kubernetes

This Timetable Management System is designed to run within a Kubernetes cluster, which provides scalability and reliability. The application is deployed and managed using various Kubernetes resources:

- **Pods:** Pods are used to run individual containers containing different components of the application.
- **Services:** Kubernetes Services allow for load balancing and expose the application to the external world.
- **Replica Sets:** Replica Sets ensure that a specified number of pod replicas are running at all times, providing high availability.
- **Deployments:** Deployments are used for declarative updates to the application, ensuring that the desired state is maintained.
- **Config Maps:** Config Maps are utilized for externalizing configuration data and making it available to the application.
- **Secrets:** Secrets are used to store sensitive information such as API keys and database credentials securely.
- **Namespaces:** Namespaces help in organizing and isolating resources within the cluster.
- **Stateful Sets:** Stateful Sets are used when state preservation and ordered deployment are required.

### Deployment Manifests

The Kubernetes deployment manifests (YAML files) for this project can be found in the `ttms-eks` directory. You can use these manifests to deploy the Timetable Management System within your Kubernetes cluster.

### Namespace

The application is deployed within its own namespace to provide isolation and better resource management.

### Secrets and Config Maps

Sensitive data and configuration settings are managed using Kubernetes Secrets and Config Maps to ensure security and flexibility.

Please refer to the [kubernetes/README.md](kubernetes/README.md) file for detailed instructions on deploying and managing this application within a Kubernetes cluster.
