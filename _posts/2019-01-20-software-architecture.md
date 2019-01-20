---
title: "Software architecture"
date: 2019-01-20
tags: [software architecture, architecture patterns]
header:
  overlay_image: "/assets/images/plitvice_full.jpg"
  show_overlay_excerpt: false
---

## Software architecture

"The software architecture is the structure or structures of the system, which comprise software elements, the externally visible properties of those elements and the relationships among them" (Len Bass)

## Recommended books

* No silver bullet (Paper by Frederick P. Brooks Jr, 1986) ([link](http://www.cs.nott.ac.uk/~pszcah/G51ISS/Documents/NoSilverBullet.html))
* Software Architecture: Foundations, Theory and Practice (Taylor, 2009)
* Software Architecture for Developers (Simon Brown, 2012)
* Patterns of Enterprise Application Architecture (Fowler, 2002)


## No Silver Bullet: Essence and Accidents of Software Engineering

* Essential Difficulties ("the difficulties inherent in the nature of software"):
	* Complexity
	* Conformity "...much complexity comes from conformation to other interfaces"
	* Changeability
	* Invisibility "Software is invisible and unvisualizable."

* Accidental Difficulties ("difficulties that today attend its production but are not inherent")

## Architecture styles

* Call and return
	* Main program and subroutine architecture

  ![Main program and subroutine]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Main_program_subroutine.png){:class="align-center"}

	* Remote procedure call architecture

  ![Remote procedure call]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Remote_procedure_call.png){:class="align-center"}

	* Object-oriented architectures

  ![Object oriented]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Object_oriented.png){:class="align-center"}

	* Layered architectures

  ![Layered]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_layers.png){:class="align-center"}

* Data-flow
	* Batch Sequential

  ![Sequential]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Data-flow_Batch_Sequential.png){:class="align-center"}

	* Pipe and Filter

  ![Pipe and Filter]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Data-flow_Pipe_Filter.png){:class="align-center"}

	* Process Control

		The data is neither batched sequential nor pipelined stream. The flow of data comes from a set of variables, which controls the execution of process. It decomposes the entire system into subsystems or modules and connects them.

* Data-centered
	* Blackboard

  ![Blackboard]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Data-centered_Blackboard.png){:class="align-center"}

	* Repository

  ![Repository]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Data-centered_Repository.png){:class="align-center"}

	* Expert system rule-based

  ![Expert system]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Data-centered_Expert_system.png){:class="align-center"}

* Independent components
	* Implicit invocation

  ![Implicit]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Independent_components_implicit.png){:class="align-center"}

	* Explicit invocation

  ![Explicit]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Independent_components_explicit.png){:class="align-center"}

## Architecture patterns categories

* Monolithic Architecture Patterns
	* Advantages:
		* Efficiency
		* Modifiability
		* Testability
		* Learnability

* Distributed Architecture Patterns
	* Advantages:
		* Modularity
		* Availability
		* Performance
		* Adaptability


## Architecture patterns

* MVC

	![MVC]({{site.url}}{{site.baseurl}}/assets/images/MVC.png){:class="align-center"}

* Layered Pattern

	![Layered]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_layers.png){:class="align-center"}

* Microkernel - plug-in

	![Microkernel]({{site.url}}{{site.baseurl}}/assets/images/Microkernel_plug-in.png){:class="align-center"}

* CQRS

	![CQRS]({{site.url}}{{site.baseurl}}/assets/images/CQRS.png){:class="align-center"}

* Event-driven

	![Event-driven]({{site.url}}{{site.baseurl}}/assets/images/Architecture_styles_Independent_components_implicit.png){:class="align-center"}

* Microservices

	![Microservices]({{site.url}}{{site.baseurl}}/assets/images/Microservices.png){:class="align-center"}

* Domain-driven

	![Domain-driven]({{site.url}}{{site.baseurl}}/assets/images/Domain-driven.png){:class="align-center"}

* Hexagonal

	![Hexagonal]({{site.url}}{{site.baseurl}}/assets/images/Hexagonal.png){:class="align-center"}

* Shared-Nothing

	![Shared-Nothing]({{site.url}}{{site.baseurl}}/assets/images/Shared-Nothing.png){:class="align-center"}

* Combined


## Software quality attributes

More info about this on [so25000](http://iso25000.com/index.php/en/iso-25000-standards/iso-25010)

* Functional Suitability
	* Functional completeness
	* Functional correctness
	* Functional Appropriateness

* Security
	* Confidentiality (the system authorizes each user to see what corresponds)
	* Integrity (protect data from being accessed by not allowed internal users or external users)
	* Fact verification (relate states to actions)
	* Trace of responsibility (logs)
	* Authenticity (identify the user)

* Performance
	* Response time
	* Resource usage (CPU, RAM, Disk)
	* Capacity (maximum number of simultaneous users for example or requests)

* Compatibility
	* Interoperability (how easy it is to communicate/integrate with this system and how well documented is that communication) 
	* Coexistence (can be in the same server with other systems?)

* Usability UX/UI
	* Recognition of suitability (is suitable for the target niche?)
	* Learning curve
	* Operability (how many steps you need to do to achieve a goal)
	* Error protection (validation of data, giving feedback to the user on data with errors)
	* Interface aesthetics
	* Accessibility (Adhesion to standards, our system can be used by people with disabilities)

* Reliability
	* Maturity (how much does the system fail under normal use? , average time between failures)
	* Availability
	* Fault tolerance (the system can continue running even if it is faulty)
	* Recoverability

* Maintainability
	* Modularity
	* Reusability
	* Analysability
	* Modificability
	* Testability (Unit tests, Integration tests and Static analysis of code)

* Portability
	* Adaptability
	* Installability
	* Replaceability

