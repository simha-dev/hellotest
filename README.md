# About this action

This is a test action. Do not use this in a workflow sadf sadf dsaf

## Quickstart

    Choose Add to workflow to add the action code to the workflow.
    Choose Visual to open the visual editor.
    Complete the mandatory fields on the Inputs, Configuration, and Outputs tabs. For details on each field, see the Additional resources section below.
    Save, validate, and commit.
    Run the action.



## Workflow examples

The following example workflow shows the Hello World Test action in use.

Workflow 1: Simple workflow

Name: Hello_WorldWorkflow
SchemaVersion: 1.0
Triggers:
- Type: Push
  Branches:
    - main
Actions:
  HelloWorldAction:
    Identifier: aws/hello-world-test-gamma@v1
    Inputs:
      Sources:
        - WorkflowSource
    Configuration:
      Parameters:
        who-to-greet: Jack Sparrow!
