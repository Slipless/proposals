# proposals

Project Planning and discussions

SLEEPLESS ENGINE:- API DESIGN PROPOSAL.

"A Progressive Designed Documentation Engine for a process driven development".

Oyegoke Abiodun || 20th-january-2021.

The main objectives of sleepless, is to be able to document API's (or any Product),
dynamically such that the documentation and testing happens at the same time and
updates can quickly be done at a sight notice. The goal is to also to allow developers
to design the presentational elements (embed:- video, images, components, online IDE's e.t.c)
of the docs as they document accordingly.

SLEEPLESS Use Case 1:
Assuming, you have a product that allows users to create different profiles for there pets.

The simple statement above has already created about 6-7 different API's:

- Authentication API's -> Signup, Login, Reset Password.
- User Management API's -> Retrieve User, Update User, Delete User.
- Pet's Management API's -> Add Pet, Retrieve Pet, Update Pet, Delete Pet.
- Search API's -> Search across Pets and Users's.

Documenting Only Signup API Endpoint would require:

- Documentig body fields (`fullname, email and password`) and their corresponding descriptions.
- Documenting response fields (`userId, fullname and email`) and their corresponding descriptions.
- Documenting error types (error code, description, and reason) for all possible reasons.

This just get tedious on progressive endpoints where new fields are added and worse when trying to keep mutiple
developers in sync across the docs.

Why Not PostMan? (Reason's I encountered, why trying to create a custom presentational view for an API Collection).

- you can't document JSON fields except using description field with markdown.
- Most companies or products have a presentational view for there docs and postman doesn't fit that model.
- Duplicate work building custom lexers and tokenizers over the parsed collections.

Core Patterns:

- Modular (Bring In What you need via dynamic components).
- Only Browser has a requirement.
- Plugin Extensible.
- Unified Data structure that can be stored.
- Persistance Storage Option.
- Collaborative Documentation Process for teams.

Utilities:

- Ability to easily convert from JSON to Documenting Structure.

Reference Documentation Sites:

- https://stripe.com/docs
- https://www.twilio.com/docs
- https://www.twilio.com/docs/voice/make-calls :: Guides documentation with steps.
- https://sendgrid.com/docs :: Simple Home page
- https://sendgrid.com/docs/api-reference/ :: combining Defination, API explorer, Code generation and Responses.
- https://dropbox.github.io/dropbox-api-v2-explorer/#account_set_profile_photo ::API Explorer.
- https://www.dropbox.com/developers/documentation/http/documentation :: Full API descriptiosn including errors.
