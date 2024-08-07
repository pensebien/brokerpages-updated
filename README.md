## Git Flow for Project Development - BrokerGenius

1. Introduction
   This document outlines the Git Flow process for the BrokerGenius project, which involves feature development using different branches corresponding to Figma pages. The Figma design file for the project can be accessed at [Figma BrokerGenius Memorial](https://www.figma.com/file/1FKNokVp92k4BzllGr8skV/BrokerGenius-memorial-new-14-5-2023?type=design&node-id=635-64&t=njEtstspvXfypzz9-0). The project's GitHub repository is available at [BrokerGenius GitHub Repo](https://github.com/lynnie21/BrokerGenius-figma-to-html).

1. Branching Strategy
   The branching strategy for the BrokerGenius project follows the Git Flow model. It includes the following branches:

- **Main Branch**: The main branch represents the production-ready codebase for BrokerGenius. It always reflects the stable and deployable version of the project.

- **Feature Branches**: Feature branches are created for each Figma page and are named accordingly. The available feature branches for BrokerGenius are as follows:

      - `feature/Welcome`: Develop features related to the Welcome page.
      - `feature/usage`: Develop features related to the usage page.
      - `feature/upgrade`: Develop features related to the upgrade page.
      - `feature/Users`: Develop features related to the Users page.
      - `feature/dashboard`: Develop features related to the Dashboard page.

  3.0 Workflow Steps
  The following steps describe the Git Flow process for feature development in the BrokerGenius project:

  3.1. Clone the Main Repository
  To start working on the BrokerGenius project, developers should clone the GitHub repository onto their local machines using the following command:

```
git clone https://github.com/lynnie21/BrokerGenius.git
```

3.2. Create a Feature Branch
After cloning the repository, developers should create a new branch based on the main branch, corresponding to the specific Figma page they will be working on. For example:

```
git checkout -b feature/welcome
```

3.3. Develop the Feature
Developers can now make changes to the codebase that relate to the specific Figma page they are assigned. Ensure that the changes align with the design and functionality specified in the Figma file.

3.4. Commit Changes
Once the necessary changes have been made, developers should commit their changes to the feature branch using the following pattern:

```
git add .
git commit -m "Task: #[task-id] - [short task title]"
```

Replace `[task-id]` with the ID number of the task from the Project Management software and `[short task title]` with a concise title describing the task. This commit message pattern helps track the tasks associated with each commit.

To find the Task ID <task-id> for the commit message, the developer can follow these steps:

Open the Project Management tool, specifically the URL you provided (e.g., https://projectdeck.morancie.com/index.php/projects/task_view/2).
On the task view page, observe the URL in the browser's address bar.
Look for the portion of the URL that contains the Task ID. In the provided example URL, the Task ID is 2.
Use the Task ID obtained from the URL as <task-id> in the commit message when committing changes.
By following these steps, the developer can identify the Task ID from the Project Management tool and include it in the commit message for tracking purposes.

Using this example, we would have a commit message as such

```
git add .
git commit -m "Task: #2 - testing GitHub push notification"

[This portion contain bullet points of what your commit has done]
```

    A more elaborate commit would be
    ``` git commit

        ## Task: #2 - Testing Github Push Notification

        This commit test the Github push notification functionality with the new Project Management tool we have

    ```

3.5. Push the Feature Branch
To make the feature branch accessible to other team members and initiate the pull request (PR) process, developers need to push the branch to the remote repository:

```
git push origin feature/main-profile
```

3.6. Submit a Pull Request
After pushing the feature branch, developers should open a pull request on the BrokerGenius GitHub repository to merge the feature branch into the main branch. Include relevant details and a summary of the changes made.
