Perception of (in)security
- Note that everything may be broken and hacked into

## Dependability & Security
### Fault-Error-Failure Chain
![[Pasted image 20230904174057.png]]
#### Fault:
- A fault (which is usually referred to as a bug for historic reasons) is a _defect in a system_. 
- The presence of a fault in a system _may or may not lead to a failure_. 
- For instance, although a system may contain a fault, its input and state conditions may never cause this fault to be executed so that an error occurs; and thus that particular fault never exhibits as a failure.
#### Error:
- An _error is a discrepancy between_ the _intended behavior_ of a system and its _actual behavior_ inside the system boundary.
- Errors _occur at runtime_ when some part of the system enters an unexpected state due to the activation of a fault. 
- Since _errors_ are generated from _invalid states_ they are hard to observe without special mechanisms, such as debuggers or debug output to logs.

#### Failure:
- A _failure_ is an instance in time when a _system displays behavior_ that is _contrary to_ its _specification_. 
- An _error may not necessarily cause a failure_, for instance an exception may be thrown by a system but this _may be caught and handled using fault tolerance techniques_ so the overall operation of the system will conform to the specification.

## Dependability
- Is a _measure of a systems availability, reliability, maintainability_ (attributes) and others indicated in the list.
- _Attributes_ is a way to _assess the dependability_ of a system
- _Threats_ are an understanding of the things that can _affect dependability_ of a system.
- _Means_ are ways to _increase_ a systems _dependability_.
## Attributes
- Determines overall dependability of a system using qualitative or quantitative measures:
1. Availability - readiness for correct service 
2. Reliability - continuity of correct service 
3. Safety - absence of catastrophic consequences on the user(s) and the environment 
4. Integrity - absence of improper system alteration 
5. Maintainability - ability for easy maintenance (repair)

>[!info] Only Availability and Reliability are Quantifiable
## Measuring Availability
![[Pasted image 20230904210328.png]]

Where:
![[Pasted image 20230904210532.png]]

So:
![[Pasted image 20230904210740.png]]
## Measuring Reliability
![[Pasted image 20230904211342.png|400]]

And:
![[Pasted image 20230904211432.png|300]]

## Means for Protection from Faults
1. __Prevention__: Fault Prevention deals with preventing faults being introduced into a system. This can be accomplished by use of development methodologies and good implementation techniques.
2. __Removal__: Fault Removal can be sub-divided into two sub-categories: Removal During Development and Removal During Use. Removal during development requires verification so that faults can be detected and removed before a system is put into production. Once systems have been put into production a system is needed to record failures and remove them via a maintenance cycle.
3. __Forecasting__: Fault Forecasting predicts likely faults so that they can be removed or their effects can be circumvented.
4. __Tolerance__: Fault Tolerance deals with putting mechanisms in place that will allow a system to still deliver the required service in the presence of faults, although that service may be at a degraded level.

Dependability means are intended to reduce the # of failures made visible to end users of a system.
## Resilience vs. Dependability
- In general, resilience can be defined as the ability of (system/person/organization) to recover/defy/resist from any shock, insult, or disturbance. 
- In systems, Laprie et al. defined resilience as the persistence of service delivery that can justifiably be trusted, when facing changes. Changes here may refer to unexpected failures, intrusions or accidents. Changes can also be unexpected load. 
- Resilience is becoming an important service primitive for various computer systems and networks. 
- Resilience deals with conditions that are outside the design envelope whereas other dependability metrics deal with conditions within the design envelope. 
- __Putting together__: Resilience is the persistence of dependability when facing changes, i.e., The persistence of the avoidance of failures that are unacceptably frequent or severe, when facing changes.

## Essential Network and Computer Security 
![[Pasted image 20230904174404.png|350]]
### 1. Confidentiality 
- Modification requires authorization
- Protect personal proprietary info and
### 2. Integrity
- Data/Service is maintained in correct state
- Protect from unintentional and intentional attacks
- Integrity ensuring non-repudiation and authenticity
	- Non-repudiation: cannot deny data or changes 
	- Authenticity: making sure that the user is authentic
### 3. Availability
- Ensure readily access to info / database
- Use of info

## Confidentiality vs Privacy
- Controls protect against unauthorized access in hands

1. __Confidentiality:__ 
	1. Pertains to data
	2. Makes sure no unauthorized access to info

2. __Privacy:__
	1. Pertains to the people
	2. Make sure unauthorized people don't have access

## Levels of Impact
### Low
- Limited adverse effect on operations
### Moderate
- Loss is expected
- Serious adverse effect on operations
### High
- Loss is expected
- Severe or catastrophic adverse effect on operations
