 bottom line is that we use CI to reduce waste in our software-delivery process by integrating the software to the central repository at each commit, instead of spending a lot of time fixing all integrations that would otherwise accumulate over time.

 Github Flow-you create a branch called feature/name-of-feature, and you commit your changes to that branch. When you think your feature is complete, you open a pull request where you solicit feedback and have the peer review of your code. After some discussion and final approval from your team members, the pull request is accepted and the change is merged into the main branch before being deployed to production. 

 ![image](https://github.com/user-attachments/assets/fc03ea8f-3130-4789-8408-d6fc4be23475)


 CI for integration- Code validation , This entails compiling the code to the type of artifact you need for production. Errors that occur here are often compiler errors, warnings

 CI for quality control - This involves simple quality control checks, like linting the source code for readability, checking if the code has multiple duplications of the code, and ensuring the code has passed a set of maintainability metrics.This workflow is often triggered when you create a pull request, so it provides input for the reviewers and helps ensure quality in the main branch.
 
 CI for security testing- This process checks whether the software that is written is secure by default, using tools called static application security testing (SAST) and dynamic application security testing tools (DAST).This CI type is also triggered at the moment of a pull request, to ensure we don’t bring new security vulnerabilities to the main branch. can be run in a regular scedule in main branch
 
 CI for packaging- roduce the final artifacts to deliver the software to production
