# APEX Approvals

The Approvals Component allows Oracle APEX to create tasks for user approval. The APEX Approvals Component is a toolkit for implementing human approvals into your application. 

You can setup task approvers and administrators at design time or determine them dynamically at runtime based on data related to the task.

## Building Blocks

- **Task Definition**

	A **shared component** used to configure task parameters, participants, actions, and due dates. 

- **Unified Task List**

	A **page** type in the Create Page wizard used to create a summary of tasks that function like an inbox.

- **Task Details Page**

	A **page** that shows details for a specific task, which can include metadata, history, comments, and actions.

- **Human Task**

	*Human Task Create* and *Human Task Manage* are the **page processes** that create and act on the task instances in your pages.

- **APEX_APPROVAL**

	A **package** API for creating, retrieving, and managing tasks programmatically.