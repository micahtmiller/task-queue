# Overview
We've built a web platform that powers our pharmacy and one of its core services is the Task system. 

A task is a single unit of work for an employee. 
There are many types of tasks, such as responding to a patient message or updating a prescription.

# Details

An employee can get the next task they should work on, with the following requirements:
- Each employee has a role that determines the types of tasks they can complete. 
    - For example, a pharmacist can respond to a patient message or update a prescription, but a customer service representative can only respond to a patient message.
- Every type of task has its own degree of urgency represented as the number of minutes between when a task is created and when it should be started by an employee.
    - For example, the urgency for responding to a patient message could be 30 minutes. If a new task to respond to a patient message is created at 2:00pm, that task should be started by 2:30pm. An employee should get the task that is closest to exceeding its start-by time.

# Deliverable

Given an employee and a collection of tasks, your challenge is to write the code for a method that returns the correct task for that employee. By the end, you should have running code that you can show meets the requirements with functional examples or tests.