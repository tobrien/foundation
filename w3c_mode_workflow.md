Patent Workflow for Working Groups Operating Under Patent Policy Option 4: W3C Mode
===================================================================================

Workflow Overview
-----------------

In order to meet our patent requirements the following workflow has been outlined. All FOCUS working groups working under Patent Policy Option 4: W3C Mode must follow this workflow.

![Document Release Workflow](images/FOCUS_Document_Release_Workflow_v1.0.3.png?raw=true "Document Release Workflow")

Git Repository Configuration
------------------

In order to abide by the requirements set out in the "Patent Policy Option 4: W3C Mode" of the project charter, the following workflow has been outlined.

Working group repos will have the following standard branches:

Git branches as they relate to the "Deliverable Development Process" in Appendix A of the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf).

* Topic and Bugfix branches (Equal to the "Pre-Draft" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf))
* `working_draft` (Equal to the "Draft Deliverable" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf))
* `candidate_recommendation` (Equal to the "Working Group Approval" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf))
* `main` (Equal to the "Approved Deliverable" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf))

Pull requests opened from the `working_draft` branch to the `candidate_recommendation` branch are equal to the "Working Group Approval" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf).
Pull requests opened from the `candidate_recommendation` branch to the `main` branch are equal to the "Final Approval" in the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf).


Git tags using [Semantic Versioning 2.0](https://semver.org/spec/v2.0.0.html) will be used to mark the official releases.

![Git Workflow](images/FOCUS_GIT_Workflow_v1.0.3.png?raw=true "Git Workflow")

All development work will be completed in the `working_draft` branch or in topic branches that are strictly merged back into the `working_draft` branch. When the specification hits development milestones and is ready to released a pull request is raised from the `working_draft` branch into the `candidate_recommendation` branch. This pull request is reviewed by the working_group before it is approved and merged by the Working Group Chair. 

Once a working group milestone has been reached for release a pull request is merged into the `candidate_recommendation` branch upon approval by the Working Group Chair. The Joint Development Foundation Projects, LLC, FinOps Open Cost and Usage Specification (FOCUS) Project has decided to have a hold period of 30 days for content that is in the Working Group Approval state before progressing to Final Approval in order to allow members to provide exclusions on essential claims prior to the adoption of a Draft Deliverable as an Approved Deliverable. No contributions that have not been held in the `candidate_recommendation` branch can be progressed into the `main` branch. 

As per the [project charter](https://github.com/FinOps-Open-Cost-and-Usage-Spec/foundation/blob/main/FOCUS_-_Membership_Agreement_Package_for_use.pdf) any exclusions on essential claims must be made to the FOCUS working group chair prior to adoption of a Draft Deliverable as an Approved Deliverable, this can be achieved via email on (focus@finops.org). Any exclusions of essential claims will be associcated with a GitHub Issue ticket and all tickets must be resolved before a pull request is able to be raised from the `candidate_recommendation` branch into the `main` branch.

The Steering Committee will review and confirm any exclusions on essential claims have been resolved before the pull request is merged into `main`. Upon approval by the Steering Committee content will be merged into the `main` branch. Each merge into `main` will be tagged with a [Semantic Versioning 2.0](https://semver.org/spec/v2.0.0.html) tag. This will make it easily possible to switch to each previous version of the specification.

Minor corrections which do not materially change the document, such as:

* Spelling mistakes
* Miss labeled figures
* Spacing issues

Can be corrected via branch, pull request and merge. This is to avoid having to do the full release cycle to make these minor corrections.
