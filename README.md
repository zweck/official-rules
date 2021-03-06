# FIGSA Official Ruleset

Many changes, including spelling fixes and wording improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put through a
bit of a design process and produce a consensus among the FIGSA committee.

The "RFC" (request for comments) process is intended to provide a consistent
and controlled path for new rules to enter the game so that all stakeholders 
can be confident about the direction the
game is evolving in.

## Table of Contents
[Table of Contents]: #table-of-contents

  - [Table of Contents]
  - [Before creating an RFC]
  - [What the process is]
  - [The RFC life-cycle]
  - [Reviewing RFCs]
  - [RFC Postponement]
  
## Before creating an RFC
[Before creating an RFC]: #before-creating-an-rfc

A hastily-proposed RFC can hurt its chances of acceptance. Low quality
proposals, proposals for previously-rejected rules, or those that don't fit
into the near-term roadmap, may be quickly rejected, which can be demotivating
for the unprepared contributor. Laying some groundwork ahead of the RFC can
make the process smoother.

Although there is no single way to prepare for submitting an RFC, it is
generally a good idea to pursue feedback from other FIGSA members
beforehand, to ascertain that the RFC may be desirable; having a consistent
impact on the game requires concerted effort toward consensus-building.

As a rule of thumb, receiving encouraging feedback from long-standing project
developers, and particularly members of the relevant [sub-team] is a good
indication that the RFC is worth pursuing.

## What the process is
[What the process is]: #what-the-process-is

In short, to get a major rule added to GiphySnap, one must first get the RFC
merged into the RFC repository as a markdown file. At that point the RFC is
"active" and may be implemented with the goal of eventual inclusion into GiphySnap.

  - Fork the RFC repo [RFC repository]
  - Copy `0000-template.md` to `text/0000-my-rule.md` (where "my-rule" is
    descriptive. don't assign an RFC number yet).
  - Fill in the RFC. Put care into the details: RFCs that do not present
    convincing motivation, demonstrate understanding of the impact of the
    design, or are disingenuous about the drawbacks or alternatives tend to be
    poorly-received.
  - Submit a pull request. As a pull request the RFC will receive design
    feedback from the larger community, and the author should be prepared to
    revise it in response.
  - Build consensus and integrate feedback. RFCs that have broad support are
    much more likely to make progress than those that don't receive any
    comments. Feel free to reach out to the RFC assignee in particular to get
    help identifying stakeholders and obstacles.
  - FIGSA members will discuss the RFC pull request, as much as possible in the
    comment thread of the pull request itself. Offline discussion will be
    summarized on the pull request comment thread.
  - RFCs rarely go through this process unchanged, especially as alternatives
    and drawbacks are shown. You can make edits, big and small, to the RFC to
    clarify or change the design, but make changes as new commits to the pull
    request, and leave a comment on the pull request explaining your changes.
    Specifically, do not squash or rebase commits after they are visible on the
    pull request.
  - At some point, a member of the team will propose a "motion for final
    comment period" (FCP), along with a *disposition* for the RFC (merge, close,
    or postpone).
    - This step is taken when enough of the tradeoffs have been discussed that
    the team is in a position to make a decision. That does not require
    consensus amongst all participants in the RFC thread (which is usually
    impossible). However, the argument supporting the disposition on the RFC
    needs to have already been clearly articulated, and there should not be a
    strong consensus *against* that position outside of the team. Team
    members use their best judgment in taking this step, and the FCP itself
    ensures there is ample time and notification for stakeholders to push back
    if it is made prematurely.
    - For RFCs with lengthy discussion, the motion to FCP is usually preceded by
      a *summary comment* trying to lay out the current state of the discussion
      and major tradeoffs/points of disagreement.
    - Before actually entering FCP, *all* members of the subteam must sign off;
    this is often the point at which many team members first review the RFC
    in full depth.
  - The FCP lasts ten calendar days, so that it is open for at least 5 business
    days. This way all
    stakeholders have a chance to lodge any final objections before a decision
    is reached.
  - In most cases, the FCP period is quiet, and the RFC is either merged or
    closed. However, sometimes substantial new arguments or ideas are raised,
    the FCP is canceled, and the RFC goes back into development mode.

## The RFC life-cycle
[The RFC life-cycle]: #the-rfc-life-cycle

Once an RFC becomes "active" then authors may implement it and submit the
rule as a pull request to the FIGSA repo. Being "active" is not a rubber
stamp, and in particular still does not mean the rule will ultimately be
merged; it does mean that in principle all the major stakeholders have agreed
to the rule and are amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is "active"
implies nothing about what priority is assigned to its implementation, nor does
it imply anything about whether a FIGSA member has been assigned the task of
implementing the rule. While it is not *necessary* that the author of the
RFC also write the implementation, it is by far the most effective way to see
an RFC through to completion: authors should not expect that other project
developers will take on responsibility for implementing their accepted rule.

Modifications to "active" RFCs can be done in follow-up pull requests. We
strive to write each RFC in a manner that it will reflect the final design of
the rule; but the nature of the process means that we cannot expect every
merged RFC to actually reflect what the end result will be at the time of the
next major rule change.

In general, once accepted, RFCs should not be substantially changed. Only very
minor changes should be submitted as amendments. More substantial changes
should be new RFCs, with a note added to the original RFC. Exactly what counts
as a "very minor change" is up to the team to decide.

## Reviewing RFCs
[Reviewing RFCs]: #reviewing-rfcs

While the RFC pull request is up, the shepherd may schedule meetings with the
author and/or relevant stakeholders to discuss the issues in greater detail,
and in some cases the topic may be discussed at a team meeting. In either
case a summary from the meeting will be posted back to the RFC pull request.

The team makes final decisions about RFCs after the benefits and drawbacks
are well understood. These decisions can be made at any time, but the team
will regularly issue decisions. When a decision is made, the RFC pull request
will either be merged or closed. In either case, if the reasoning is not clear
from the discussion in thread, the team will add a comment describing the
rationale for the decision.

## RFC Postponement
[RFC Postponement]: #rfc-postponement

Some RFC pull requests are tagged with the "postponed" label when they are
closed (as part of the rejection process). An RFC closed with "postponed" is
marked as such because we want neither to think about evaluating the proposal
nor about implementing the described rule until some time in the future, and
we believe that we can afford to wait until then to do so. Historically,
"postponed" was used to postpone rule changes. Postponed pull
requests may be re-opened when the time is right. We don't have any formal
process for that, you should ask members of the relevant team.

Usually an RFC pull request marked as "postponed" has already passed an
informal first round of evaluation, namely the round of "do we think we would
ever possibly consider making this change, as outlined in the RFC pull request,
or some semi-obvious variation of it." (When the answer to the latter question
is "no", then the appropriate response is to close the RFC, not postpone it.)
