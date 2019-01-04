# Stack-Agnostic questions

This document contains questions which apply to any technology. You are supposed to choose and ask some questions according to the candidate's experience and target position.

## Index

General questions
Questions which every software engineer must be able to answer

Full-stack
For full-stack engineer positions

Back-end
Full-stack or back-end engineer positions

Front-end
Full-stack or front-end engineer positions

# General questions

These are questions which every software engineer must be able to answer.

- Are you familiar with **Git**?
- Are you familiar with the basic bash commands?
- Are you familiar with **Docker**?
- What is the TDD methodology?
- What is the Continuous Integration?

# Full-stack

If the candidate is applying for a **full-stack engineer** position, you must ask them one open question. It requires them to pick the potential technology which they hold to be the best for the given purpose.

## 1. List of people app

##### Question:

Let's say you have to build an application to manage a list of people. The user should be able to see the list, and to add, remove and delete a person from it. You are free to choose your favorite language(s), or the one you think it's more appropriate, database and architecture. What approach would you use for doing it?

#### Extra points

- Single stack for both back-end and front-end
- Client-server architecture
- Front-end using React, Angular or Vue
- Focus on security best practices
- Focus on data structure
- Focus on database technology
- Consider data validation
- Consider design and user experience
- Consider the possibility the project will increase its size

#### Red flags

- Not considering a SPA (Single Page Application)
- Choose obsolete technologies (for example, anything which runs on Tomcat)
- Pick a monolithic architecture
- Can't explain the reason of the chosen stack
- Takes too long to provide a solution

# Back-End

The following questions can be asked to candidates who are applying for either a **full-stack** or a **back-end engineer** position. They are organized by difficulty, so depending on the candidate's experience you might want to ask some basic or some advanced questions.

## Basic

**How do you prevent SQL injections when dealing with a relational database?**

> The right way to prevent SQL injections is to use a db driver which supports parameters binding, or to sanitize the user input (less secure).

**What is the difference between POST and PUT methods?**

> In RESTful services, POST is used to create a resource, while PUT is used to update it.

## Advanced

**What is the difference between PUT and PATCH methods?**

> Even though PATCH is not used as widely as PUT, both methods are used to update a resource. When updating a resource with a PUT request, you have to send the full payload as the request body. With PATCH, you only need to send the parameters which you want to update.

# Front-End

The following questions can be asked to candidates who are applying for either a **full-stack** or a **front-end engineer** position. They are organized by difficulty, so depending on the candidate's experience you might want to ask some basic or some advanced questions.

## Basic

**What is the difference between a container and a presentational component?**

> The containers (aka stateful or smart) components are concerned on _how things work_. Most of the times they are pages, or components which deal with data. They pass data down to their children components.

> The presentational (aka stateless or dumb) components are concerned on _how things look_.

## Advanced

**Why is immutability important?**

> Immutability is important to increase predictability and performance. Predictability, because mutation might create unexpected side effects. And performance, because it avoids tracking every state change. While creating new objects every time might sound inefficient, it is actually very efficient as the garbage collector takes care of cleaning not used references.
