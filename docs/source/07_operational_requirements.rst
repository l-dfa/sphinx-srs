
.. _operational_requirements:

Operational Requirements
========================

Provide the operational requirements in this section. Operational requirements describe how the
system will run and communicate with operations personnel.

Do not state how these requirements will be satisfied. For example, in the Reliability section,
answer the question, “How reliable must the system be?” Do not state what steps will be taken
to provide reliability. The rules for stating requirements, outlined in Section 4.1, also apply to
these requirements.

Distinguish preferences from requirements. Requirements are based on business needs.
Preferences are not. If, for example, the user expresses a desire for sub-second response but does
not have a business-related reason for needing it, that desire is a preference.

Other applicable requirements on system attributes may be added to the list of subsections
below. If there is a ConOps for the system or application, all subsections listed in Section 6 of
the ConOps document must be addressed in Section 7 of the SRS.

Security
------------------

The Security Section describes the need to control access to the data. This includes controlling
who may view and alter application data. Use the following criteria:

* State the consequences of the following breaches of security in the subject application:

  * Erasure or contamination of application data
  * Disclosure of Government secrets
  * Disclosure of privileged information about individuals
  
* State the type(s) of security required. Include the need for the following as appropriate:

  * State if there is a need to control access to the facility housing the application.
  * State the need to control access by class of users. For example, “No user may access any
    part of this application who does not have at least a (specified) clearance.”
  * State the need to control access by data attribute. State, for example, if one group of
    users may view an attribute but may not update it while another type of user may update
    or view it.
  * State the need to control access based on system function. State, for example, if there is a
    need to grant access to certain system functions to one type of users, but not to others.
    For example, "The system shall make Function N available to the System Administrator
    only."
  * State if there is a need for accreditation of the security measures adopted for this
    application. For example, C2 protection must be certified by an independent authorized
    organization.

Audit Trail
-------------

List the activities that will be recorded in the application’s audit trail. For each activity, list the
data to be recorded.

Data Currency
-----------------

Data currency is a measure of how recent data are. This section answers the question, “When the
application responds to a request for data, how current must the data be?” Answer that question
for each type of data request.

Reliability
------------------

Reliability is the probability that the system will be able to process all work correctly and
completely without being aborted. Reliability is evaluated as follows:

* State the following in this section:

  * What damage can result from failure of this system?
  
    * Loss of human life
    * Complete or partial loss of the ability to perform a mission-critical function
    * Loss of revenue
    * Loss of employee productivity
    
  * What is the minimum acceptable level of reliability?
  
* State required reliability in any of the following ways:

  * Mean Time Between Failure is the number of time units the system is operable before the
    first failure occurs.
  * Mean Time To Failure is computed as the number of time units before the system is
    operable divided by the number of failures during the time period.
  * Mean Time To Repair is computed as the number of time units required to perform
    system repair divided by the number of repairs during the time period.

Recoverability
---------------

Recoverability is the ability to restore function and data in the event of a failure.
Answer the following questions in this section:

* In the event the application is unavailable to users (down) because of a system failure, how
  soon after the failure is detected must function be restored?
* In the event the database is corrupted, to what level of currency must it be restored? For
  example “The database must be capable of being restored to its condition of no more than
  1 hour before the corruption occurred.”
* If the processing site (hardware, data, and onsite backup) is destroyed, how soon must the
  application be able to be restored?

System Availability
-----------------------

System availability is the time when the application must be available for use. Required system
availability is used in determining when maintenance may be performed.

In this section, state the hours (including time zone) during which the application is to be
available to users. For example, “The application must be available to users Monday through
Friday between the hours of 6:30 a.m. and 5:30 p.m. EST.” If the application must be available
to users in more than one time zone, state the earliest start time and the latest stop time.
Include the times when usage is expected to be at its peak. These are times when system
unavailability is least acceptable.

Fault Tolerance
------------------

Fault tolerance is the ability to remain partially operational during a failure. Describe the
following in this section:

* Which functions do not need to be available at all times?
* If a component fails, what (if any) functions must the application continue to provide?
* What level of performance degradation is acceptable?

For most applications, there are no fault tolerance requirements. When a portion of the
application is unavailable, there is no need to be able to use the remainder of the application.

General Performance
---------------------

Describe the requirements for the following:
* Response time for queries and updates
* Throughput
* Expected rate of user activity (for example, number of transactions per hour, day, or month)
  Specific performance requirements related to a specific functional requirement should be listed
  with that functional requirement (see Section 4.1 for guidance).
  
Capacity
---------------

List the required capacities and expected volumes of data in business terms. For example, state
the number of cases about which the application will have to store data. For example, “The
system shall be able to process a projected volume of 600 applications for naturalization per
month.” State capacities in terms of the business. Do not state capacities in terms of system
memory requirements or disk space.

Data Retention
-----------------

Describe the length of time the data must be retained. For example, “Information about an
application for naturalization shall be retained in immediately accessible form for 3 years after
receipt of the application.”
