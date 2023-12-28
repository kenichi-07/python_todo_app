# python_todo_app
This is a CI/CD project for a To-Do list application. 

We have taken the following steps to create this project:

1. We created this repository.
2. We created 3 environments: dev, test and prod.
3. We cloned this repository to local terminal and written a python code for a small to-do-list application.
4. Now we pushed the code to dev env.
5. We installed Jenkins.
6. Created new access_key token for using Github API for jenkins with permission of repository and workflow.
7. Configured Github credentials in Jenkins.
8. Now we create a new job in Jenkins as a freestyle project and name it as to-do-list.
9. Select the source code as Git and provided the link of repository.
10. In "build step" we provide a shell command python3 to_do_v1.py
11. Apply changes and save this ci/cd project.
12. Run the pipeline.
