This workflow uses Adaptive Approvals to create a parallel approval policy that contains:

Manager
Manager_Plus_One  (Identity's Manager's Manager).

This workflow works in conjunction with the Manager_Plus_One transforms that can also be found in CoLab (https://developer.sailpoint.com/discuss/c/colab/colab-transforms)


Workflow does the following:

1. Triggers on Access Request Submitted
2. Gets Identity data for the RequestFor ID
3. Creates Approval Policy
   a. Multi-Step Approval Type
   b. Parallel Approval Schema
   c. Reviewers
     - Manager
     - Identity (Other) - Choose Variable: $.getIdentity.attributes.managerPlusOneIscId
