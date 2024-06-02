---
title: Overview - tech-oriented-mastery
created: 2024-06-01 01:22
tags:
  - programming
  - projects
  - web-development
status: ongoing
---
# tech-oriented-mastery

## Overview
---
**Project Name:** tech-oriented-mastery
**Description:** Utilizing AI to assist and engage developers on programming knowledge & skills.
**Objectives:** 
1. Users can select a category to be tested on.
2. A chatbot will interact and prompt questions to the user.
3. The chatbot will respond with answers, definitions, analysis, etc..., it will also provide performance review at the end of an interview.

## ~~Project Details~~
---
**~~Client~~:** 
**~~Stakeholders~~:** 
~~**Team Members~~:** 

## Timeline
---
**Start Date:** 06/01/2024
**End Date:** 07/01/2024
**Task Estimates:** 
- front-page: ~2 Days
	- Design and implement a main front page.
	- Utilize interactive 3d models.
- interview-categories: 4 Hours
	- 

## Requirements
---
**Functional Requirements:** 
1. <u>User Interaction</u>
	- User must be able to select testing categories.
	- Allow user to select multiple responses for an answer (in case of ai hallucinations, i.e. 2-3 responses per prompt per chatgpt )

2. <u>Testing Categories</u>

	Terminology:
	- Chatbot provides basic to advanced technical and coding terms tailored to mid-level software developers and below and will provide definitions, explanations, and short examples after the user answers.
	
	Code Snippet Explanations:
	- Chatbot will provide user with a code snippet.
	- The snippet can be one of these things:
		1. Explain the snippet's main function.
		2. Point out an error within a snippet.
		3. Fill in a missing line to get correct code.
	
	Code Demonstrations:
	- Chatbot will provide a prompt for the user to perform a coding demonstration.
	- The demonstration ETA shouldn't be longer than 30 min to complete.
	- Chatbot will provide review and analysis.

	Technical Interviews:
	- The chatbot should be able to conduct a simulated technical interview, asking questions and evaluating user responses.
	- Users should receive feedback on their answers, including correct answers and explanations.

3. <u>User Authentication</u>
	- Users should have the ability to start a new session, or continue from a previous session.

**Non-Functional Requirements:** 
1. Usability
	- The chatbot interface should be intuitive and easy to navigate.
	- Users should find it easy to start a session, select categories, and receive information.
2. Reliability
	- The system should include mechanisms for auto-recovery in case of failure (e.g., reconnecting sessions, saving state periodically).
3. Maintainability
	- Automated tests (unit, integration, and end-to-end) should cover major functionalities to ensure reliability during updates.

## Design
---
**Wireframes:** [[Wireframes - tech-oriented-mastery]]
**~~Mockups~~:** 
**UI/UX Notes:** 
- Color scheme:
- Typography:
	- Font Family:
		- Headings:
		- Body:
	- Font Sizes:
	- Font Weights:
- Breakpoints:

## Development
---
**Technology Stack:**
- Frontend: TypeScript, React, React Three Fiber
- Backend: Nodejs
- Database: postgreSQL
- Other: OpenAI API
**Architecture:** 
**Setup Instructions:** 
1. Clone repository
```
git clone https://github.com/AndrewKohn/tech-oriented-mastery.git
```
2. Install dependencies: `npm install`
3. Apply tokens to the `server/.env` file
4. Run live server: `npm run dev`

## Code Repositories
---
**Frontend Repository:** [https://github.com/AndrewKohn/tech-oriented-mastery](https://github.com/AndrewKohn/tech-oriented-mastery)
**Backend Repository:** [https://github.com/AndrewKohn/tech-oriented-mastery](https://github.com/AndrewKohn/tech-oriented-mastery)
**Other Repositories:** 

## Testing
---
**Test Plan:** 
**Unit Tests:** 
**Integration Tests:** 
**End-to-End Tests:** 

## Deployment
---
**Deployment Instructions:** 
**Environment Configurations:**
- Development: 
- Staging: 
- Production: 
**CI/CD Pipeline:** 

## Documentation
---
**User Guide:** 
**API Documentation:** 
**Developer Documentation:** 

## Issues and Tracking
---
**Issue Tracker:** 
**Known Issues:** 
**Feature Requests:** 

## Notes
---
**Meeting Notes:** 
**Decision Log:** 
**Miscellaneous:** 

## Resources
---
**References:** 
**Learning Materials:** 