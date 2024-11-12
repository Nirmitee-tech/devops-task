# DevOps Engineer Hiring Task

Welcome! This assignment is designed to showcase your skills in building, deploying, and managing applications in Kubernetes and cloud-native environments.

## Goal

Demonstrate your ability to:
1. Containerize applications.
2. Deploy them in a Kubernetes environment.
3. Set up a continuous delivery (CD) pipeline with cloud-native tools.

## Task Overview

You will accomplish the following:

1. **Kubernetes Test Cluster Setup**
   - Build a small Kubernetes test cluster, either locally (using tools like **Minikube** or **Kind**) or in the cloud.
   - A single-node cluster is sufficient, but feel free to expand as needed.
   
2. **Application Containerization**
   - Create Dockerfiles for the provided applications (`app_a` and `app_b`), ensuring they run correctly in their containers and return expected results.
   
3. **Deployment Mechanism in Kubernetes**
   - Develop a repeatable deployment mechanism for both applications within Kubernetes.
   
4. **Continuous Delivery Plan**
   - Outline a CD plan for these applications. Specify the tools/vendors you would consider and your evaluation criteria for choosing them.

## Deliverables

Create a GitHub repository with the following:

1. **Dockerfiles for Each Application**  
   - Separate Dockerfiles for `app_a` and `app_b`.
   
2. **Repeatable Deployment Mechanism**  
   - A deployment script (e.g., `deploy.sh`) or Kubernetes configuration files (e.g., YAML manifests) for deploying each application.

3. **Documentation**  
   - A **README.md** with setup instructions so we can run the applications ourselves.
   - A short document (e.g., `CD_Plan.txt`) outlining:
     - Your continuous delivery plan.
     - Your chosen tools and the rationale behind each choice.

4. **Commit History**  
   - Meaningful and well-organized git commit messages to demonstrate your approach.
   - Each commit should describe its purpose and changes clearly.

---

## Bonus Points

To stand out, consider adding any of the following:

- **Multi-stage Docker Builds**: Separate stages in Dockerfiles for building and running the applications.
- **Automated Kubernetes Environment**: Script or configuration for an automated setup of a local or cloud-based Kubernetes environment.

---

## Submission

1. **Repository**: Create a new GitHub repository with a unique name for this assignment.
2. **Privacy**: If you prefer, keep the repository private and add us as collaborators.
3. **Avoid Forks or PRs**: Do not fork this task’s repo or submit pull requests.


## Notes

- Please do not fork or submit a PR to this repo
- Feel free to change the python application code and/or their requirements to
  make them more "cloud native"
- If you get stuck or need more information, please reach out for clarity
- Have fun!

## Getting Started in Local Development

Running the apps outside of a container:

```
pip install -r requirements.txt
sqlite3 database.db < schema.sql
python app_a.py
python app_b.py
```

Making a request

```bash
# Test a non-auth'd route
curl http://127.0.0.1:5000/hello

curl -X POST -H 'Authorization: mytoken' http://127.0.0.1:5000/jobs
```
