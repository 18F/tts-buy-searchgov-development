**General Services Administration**

Federal Acquisition Service

Technology Transformation Services

1800 F St NW | Washington, DC | 20405

**Office of Products and Programs  
Search.gov Development Support Services**

**Quality Assurance Surveillance Plan**

# **Introduction**

The General Services Administration (GSA) Technology Transformation
Services (TTS) has developed this Quality Assurance Surveillance Plan
(QASP) to evaluate contractor actions while implementing the Performance
Work Statement (PWS). It is designed to provide an effective
surveillance method of monitoring contractor performance for each listed
objective on the Performance Requirements Summary in the Task Order
(TO). It also provides a systematic method to evaluate the services the
contractor is required to furnish.

# **Standard**

The contractor is responsible for management and quality control actions
to meet the terms of the TO. The contractor shall perform all work
required in a satisfactory manner in accordance with the requirements of
the PWS. The Contracting Officer's Representative (COR) shall notify the
Contracting Officer (CO) for appropriate action if it is likely that the
contractor will not achieve successful final delivery of the software
code in accordance with the performance objectives and acceptable
quality levels identified below.

# **The CO’s responsibilities**

The CO is responsible for monitoring contract compliance, contract
administration, and cost control and for resolving any differences
between the observations documented by the COR and the contractor. The
CO will designate a COR as the Government authority for performance
management. The number of additional representatives serving as
technical inspectors depends on the complexity of the services measured,
as well as the contractor’s performance, and must be identified and
designated by the CO.

# **The COR’s responsibilities**

The contracting officer’s representative (COR) is designated in writing
by the CO to act as his or her authorized representative to assist in
administering a contract. COR limitations are contained in the written
appointment letter. The COR is responsible for technical administration
of the project and ensures proper Government surveillance of the
contractor’s performance. The COR is not empowered to make any
contractual commitments or to authorize any contractual changes on the
Government’s behalf. Any changes that the contractor deems may affect
contract price, terms, or conditions shall be referred to the CO for
action. The COR will have the responsibility for completing QA
monitoring forms used to document the inspection and evaluation of the
contractor’s work performance. Government surveillance may occur under
the inspection of services clause for any service relating to the
contract.

# **Performance Requirements Summary**

The COR will evaluate the performance objectives through surveillance as
reflected below by reviews and acceptance of work products and services.
As indicated, the COR will assess progress towards the final delivered
software code. The performance requirements listed below are required
for every sprints to enable incremental delivery of code. Code will be
assessed by the Government to ensure that the contractor is on a path to
successful final
delivery.

## 

| **Characteristic**    | **Performance Standard(s)**                                                                                                                                                                                                                                                           | **Acceptable Quality Level**                                                                                                                                                                                                                                                                  | **Method of Surveillance**                                                                                                     |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Tested Code           | Code delivered under the order must have comprehensive test code coverage and a clean code base                                                                                                                                                                                       | 100% test coverage of all relevant code, including all existing tests and any new tests that may be needed                                                                                                                                                                                    | Combination of manual review and the results of automated testing by Government personnel (TTS)                                |
| Accepted              | Functions agreed upon as the Definition of Done for a given user story                                                                                                                                                                                                                | All functions appear and operate as expected                                                                                                                                                                                                                                                  | Manual review of Government personnel (TTS) for user-facing features and bugs. Some user stories can be accepted by developers |
| Accessible            | Web Content Accessibility Guidelines 2.0 AA (WCAG 2.0 AA) standards                                                                                                                                                                                                                   | 0 errors reported for WCAG 2.0 AA standards using an automated scanner and 0 errors reported in manual testing                                                                                                                                                                                | http://wave.webaim.org/extension/ and manual review by Government personnel (TTS)                                              |
| Deployed              | Code must successfully build and deploy                                                                                                                                                                                                                                               | Three logically-isolated environments: (1) development; (2) staging (representative of the production environment); and (3) production                                                                                                                                                        | Combination of manual review and automatic testing by Government personnel (TTS).                                              |
|                       | Minimal outage time for production pushes                                                                                                                                                                                                                                             | Non-database deployments take less than one minute                                                                                                                                                                                                                                            | Manual review of deployment                                                                                                    |
| Documentation         | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided as appropriate to the release | In order to meet TTS needs as agreed to following initial releases with the Product Owner, COR, and CO                                                                                                                                                                                        | Combination of manual review and automatic testing, if available, by Government personnel (TTS)                                |
| Secure                | Participate in GSA’s security scanning, monitoring, and authorization activities                                                                                                                                                                                                      | Remediation of critical or high issues within 30 days and moderate issues within 90 days                                                                                                                                                                                                      | Review by GSA IT                                                                                                               |
| System Infrastructure | Low latency                                                                                                                                                                                                                                                                           | 95th percentile latency for searchers’ queries at less than 750 milliseconds and for type-ahead suggestions at less than 50 milliseconds. 95th percentile latency for administrators’ changes in the Admin Center and Super Admin to be reflected on results pages at less than three seconds | DataDog, Airbrake, Pingdom, New Relic, and Elastic Monitoring                                                                  |
|                       | High uptime                                                                                                                                                                                                                                                                           | 99.95% or higher availability                                                                                                                                                                                                                                                                 | DataDog, Airbrake, Pingdom, New Relic, and Elastic Monitoring                                                                  |
|                       | Prompt outage notification                                                                                                                                                                                                                                                            | Detect any service disruptions within two minutes                                                                                                                                                                                                                                             | Manual review of performance during outage                                                                                     |

If any deliverables produced by the contractor during performance fail
the quality levels provided above, the contractor will correct those
deliverables to meet the specified quality level at no extra cost to the
Government.
