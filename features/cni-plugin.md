[//]: # (The syntax preceeding this line is a comment marker used to help guide the author in populating this document)
[//]: # (to github. Unlike HTML comments commonly used throughout istio.io documentation, this comment will not be rendered)
[//]: # (by github. Comments must be separated by carriage return preceding and concluding the text and be a single line.)

[//]: # (This is a living document representing the maturity of a feature. Completion of this template enables Istio work groups)
[//]: # (to collect information on potential new functionality. This template should be completed before users are exposed to)
[//]: # (any new experimental feature. Please complete this template during development.)

[//]: # (The feature implementation section must be completed before submission of the document.)

# Feature:

[//]: # (All information in this section is mandatory.)

**Feature name:** Istio CNI Plugin

[//]: # (The name of the feature, e.g. Multiple control planes)

**Primary lead(s):** [Pengyuan Bian](https://github.com/bianpengyuan), [Mandar Jog](https://github.com/mandarjog)

[//]: # (The primary lead or leads responsible for the feature. These individuals serve as a point of contact for the feature.)

**Short description:** Istio CNI Plugin for handling traffic redirection to the sidecar proxy in Istio user application pods.

[//]: # (A short description of the feature. One or two sentences maximum.)

**Design Docs:**
[Istio CNI Plugin](https://docs.google.com/document/d/1B5gGvdlZEfk5oAL8Qx8NdRKDYb3YlGphJoQLhwPBXYw/edit#)
[Istio CNI Race Condition Mitigation](https://docs.google.com/document/d/1SQzrFxtcn3o_79OtJYbSHMPuqZNhR3EaEhbkpBVMXAw/edit)
[Istio CNI Upgrade Safety](https://docs.google.com/document/d/1CVRNAlDEsU6Lmssv01gWLt3uaaWJNBVLlIyZeGWh0KA/edit)

[//]: # (Design docs for feature)


**Relevant Documentation:**

[//]: # (Links to relevant documentation for feature)

*[Install Istio with the Istio CNI plugin](https://istio.io/latest/docs/setup/additional-setup/cni/)

**RFC:**

[//]: # (Link to RFC for feature)


---

## Experimental

### Requirements:

[//]: # (All information in this section is mandatory for promotion. Please modify the links in this)
[//]: # (section.)

- [ ] [User stories](insert_your_link_here) reviewed in a work group meeting.

[//]: # (User stories are a way to communicate user value. User stories follow the style)
[//]: # (as a [type of user], I want [an action] so that [a benefit/a value]. Istio currently has no user)
[//]: # (story template. Maybe you can make one?)

[//]: # (User stories must be presented in a work group meeting. They need no approval and are later integrated)
[//]: # (into the RFCs, which do need approval for alpha. You may find value to negotiate within the work group where the)
[//]: # (user stories are presented to help clarify the user stories.)

- [ ] [RFC Authored] - [create an RFC using template](https://docs.google.com/document/d/1ewJoCcw5-04crH-M0xw4zFxz1cfwVCPnNyW4K3m4Yyc/template/preview).

[//]: # (An RFC is mandatory to graduate to experimental. The RFC does not have to be reviewed in a work group)
[//]: # (meeting to graduate to experimental.)

- [ ] [Documentation](insert_your_link_here) for enabling and using the feature.

[//]: # (The documentation instructions may exist on the developer wiki or the team drive. They may include instructions)
[//]: # (for building running a `istioctl experimental command`, or using the preview profile,)
[//]: # (or any other relevant information.)

- [ ] [Feedback plan](insert_your_link_here).

[//]: # (This may include user feedback meetings, discuss.istio.io conversations, GitHub issues, or mailing lists.)

- [ ] Disabled by default.

- [ ] No impact on performance when the feature is disabled.

---

## Alpha

### Requirements: 

**Design**

- [x] RFC has been approved describing the intention of the feature as well as the user stories behind the feature. 

**Config**

- [x] Explicit user action is required to enable this feature (e.g. a config field, config resource, or installation action). 
[NET_ADMIN and NET_RAW capabilities](https://istio.io/latest/docs/ops/deployment/requirements/#pod-requirements)

> Link to instructions for enabling

**Docs**

- [x] Reference docs are published to preliminary.istio.io or the Istio wiki.
- [x] Basic feature docs are published on preliminary.istio.io describing what the feature does, how to use it, and any caveats. 
- [ ] Release notes entries added as appropriate
N/A
- [ ] Upgrade notes entries added as appropriate
N/A

**Tests**

- [x] Automated integration tests cover core use cases with the feature enabled. 
- [x] When disabled, the feature does not affect system stability or performance. 

**API**

- [x] Initial API review.

**Approvals**

- [x] The appropriate work group(s) have reviewed and approved promotion of the feature.
- [x] The TOC has reviewed and approved promotion of the feature as part of the
	roadmap for a release.

---

## Beta

### Requirements: 

**Design**

- [x] Design doc describing the intention of the feature, how it will be
	implemented, and any thoughts on how to test the feature has been approved by
	relevant work group leads
- [x] Feature coverage and test plans written and approved.

**Docs** 

- [x] Documentation on istio.io includes performance expectations; may have caveats.
- [x] Documentation on istio.io includes samples/tutorials.
- [x] Documentation on istio.io includes appropriate glossary entries.
- [x] All new documentation containing user actions includes istio.io tests.
- [x] Release notes have been added.
- [x] Upgrade notes have been added.

**Tests**

- [x] Integration tests cover feature edge cases
- [x] End-to-end tests cover samples/tutorials
- [x] Fixed issues have tests to prevent regressions
- [x] Stability/stress test suite includes coverage for the feature.

**Performance**

- [x] Tests exist with the feature enabled that can be integrated with our automated performance testing.

**API**

- [x] TOC has reviewed the API and determined it to be complete. 

**Tooling**

- [x] Any necessary tooling to use/debug the feature has been implemented and is complete. 

**Bugs**

- [x] Feature has no known major issues.

**Approvals**

- [x] The appropriate work group(s) have reviewed and approved promotion of the feature.
- [x] The supportability review panel has reviewed promotion of the feature.  
- [x] The TOC has reviewed and approved promotion of the feature as part of the
	road map for a release.

---

## Stable

### Requirements: 

**Performance**

- [ ] Latency, throughput, and scalability are quantified and documented on
	istio.io. 

**Bugs**

- [x] Feature has no known major issues. 

**Approvals**

- [ ] The appropriate work group(s) have reviewed and approved promotion of the feature.
- [ ] The supportability review panel has reviewed promotion of the feature.  
- [ ] The TOC has reviewed and approved promotion of the feature as part of the
	roadmap for a release.


