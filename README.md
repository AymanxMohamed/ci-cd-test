# Github Actions

```yml
# name: <workflow name>
name: First Workflow
# on: specify the trigger of the workflow
on: workflow_dispatch
# her we specify the list of jobs 
jobs:
  first-job:
    # ubuntu-latest is the runner machine and you get it's name from github
    # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners
    runs-on: ubuntu-latest
    # Her we specify the list of the steps in the job
    # on each step we specify the name: of the step
    #  we specify also the command to be run using the run key
    steps:
      - name: Print greeting
        run: echo "Hello world!"
      - name: Print goodbye
        run: echo "Done -bye!"
```
