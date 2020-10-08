
# SingularityNet Platform Enhancement Proposal (SNEP)

The SingularityNet Platform Enhancement Proposal is a document that describes an enhancement to the platform components. The document should provide a concise technical specification of the feature and a rationale for the feature. It should adhere to the guidelines as defined in ** &lt;link to first proposal>**. The author is expected to build consensus on the proposal and take it forward.


# Types

There are two two types of proposals

1. Standard - Proposals requiring changes to one or more components of the platform. They can be further classified as
    1. Contracts - Enhancements related to smart contracts (Either new contracts or changes to existing contracts)
    2. Components - Enhancements in the Daemon, snet-cli, SDK or any other component
2. Meta - Proposals related to documentation or the process adopted on the platform

The more focused the proposal, the more successful it's likely to be. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement. The proposed implementation, if applicable, must be solid and must not complicate the platform.

Your role as the champion is to write the proposal using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea. Following is the process that a successful SNEP will move along:


```
[ DRAFT ] -> [ LAST CALL ] -> [ ACCEPTED ] -> [ FINAL ]
```


Each status change is requested by an **author** and reviewed by the **editors.** Use a pull request to update the status. 


# Workflow

We will follow a workflow similar to that of EIPs



1. **Draft** - a proposal that is undergoing rapid iteration and changes
2. **Last Call** - a proposal that is done with its initial iteration and ready for review by a wide audience
3. **Accepted** - a proposal that has been in Last Call for at least 2 weeks and any technical changes that were requested have been addressed by the author
4. **Rejected** - a Last Call proposal that has been rejected by the core team
5. **Deferred** - a Last Call proposal that is not being considered for immediate adoption. May be reconsidered in the future
6. **Final**  - a proposal that the Core Devs have decided to implement and release or has already been released.

The editors will process these requests as per the conditions below.



1. **Draft** - Once the first draft has been merged, you may submit follow-up pull requests with further changes to your draft until such point as you believe the SNEP to be mature and ready to proceed to the next status. An SNEP in draft status must be implemented to be considered for promotion to the next status. An editor will assign Last Call status and set a review end date (review-period-end), normally 14 days later.
2. **Last Call** - The Proposal will be reviewed by the **core team**
    1. A Last Call which results in material changes or substantial unaddressed technical complaints will cause the SNEP to revert to **Draft or could be Rejected**
    2. A successful Last Call without material changes or unaddressed technical complaints will become **Accepted**.
3. **Accepted** - The proposal is taken up for implementation. When the implementation is complete and adopted by the community, the status will be changed to “Final”
4. **Final** - This proposal has been implemented


# Responsibilities


## Editors 

*   Qualified members of the community 
    *   Qualifying criteria
        *   Developers that contribute by
            *   Creating issues / enhancements on platform repos
            *   Contribute fixes to existing issues
            *   Contributes towards improved documentation
            *   Help review PRs on any of the platform repos
            *   Developers selected by other editors and core team members
*   All members of the SingularityNet platform team 


## Core Team


*   Qualified contributing (who have contributed code which has been accepted) members of the community 
*   Qualifying criteria
    *   Developers that have
        *   Contributed code which has been accepted by the core team
        *   Designed solutions that have been accepted by the core team
        *   Regularly review PRs
        *   Selected by the core team
*   All members of the SingularityNet platform team 
