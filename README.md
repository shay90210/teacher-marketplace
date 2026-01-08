# Teacher Resource Marketplace (Sinatra Prototype)

## Overview

This project is a lightweight prototype of a teacher resource marketplace built with Ruby and Sinatra. The goal of this application is to model core marketplace functionality—resource listings, categorization, and user flows—while intentionally avoiding the abstractions of a full-stack framework.

This project serves as a foundational MVP and learning-focused implementation, designed to validate application structure and domain logic before scaling to a production-ready framework.

________________________________________________________________________________

## Why Sinatra?

Sinatra was chosen deliberately for this phase of development to focus on core web fundamentals, including:

- HTTP request/response lifecycle
- Explicit routing and controller logic
- Manual MVC organization
- Server-rendered views using ERB
- Static asset serving without framework magic

By using Sinatra, this project emphasizes understanding how web applications work under the hood, rather than relying on conventions provided by larger frameworks like Ruby on Rails.

## Current Features

- Resource listings (CRUD functionality)
- Categorization and basic filtering
- Server-rendered pages using ERB templates
- Shared layouts and partials
- Static asset handling (CSS)

Clean, REST-style routes

⚠️ This prototype intentionally excludes authentication, payments, and complex authorization logic. Those concerns are planned for a future Rails implementation.

## Project Structure
```
├── app.rb
├── views/
│   ├── layout.erb
│   ├── index.erb
│   └── resources/
├── public/
│   └── css/
│       └── styles.css
└── README.md
```

- app.rb — Application entry point and routing
- views/ — ERB templates and layouts
- public/ — Static assets served by Sinatra
- README.md — Project documentation and design decisions

## Tech Stack

- Ruby
- Sinatra
- ERB
- HTML5
- CSS3

## Design Decisions

- No authentication: This phase focuses on content structure and routing clarity.
- Server-rendered views: Chosen to emphasize backend-rendered workflows and simplicity.
- Minimal dependencies: Keeps the codebase readable and easy to reason about.

These decisions allow the project to remain small, testable, and easy to refactor.

## Future Plans

This Sinatra prototype will serve as the foundation for a full Ruby on Rails rebuild, which will include:

- User authentication and roles
- Relational database modeling
- Secure uploads
- Payment processing (Stripe test mode)
- Authorization and admin features

The Rails version will address scalability and production concerns that are intentionally out of scope for this prototype.

## How To Run Locally
```
bundle install
ruby app.rb
```