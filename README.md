# Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Project Overview
This ServiceNow project automates the configuration task associated with a Standard Laptop service request.

The workflow uses **ServiceNow Flow Designer** to create a Catalog Task after the service request is approved. The task is configured with the short description **"Laptop need to Configured"**, description **"Laptop need to Configured"**, Assignment group **Hardware**, and Approval **Approved**.

## Project Objective
The project aims to:
1. Create a seamless experience for users requesting standard laptops by ensuring timely configuration.
2. Reduce manual intervention and potential errors.
3. Improve IT resource utilization through automated task allocation.
4. Enhance efficiency and productivity in IT procurement operations.

## Technology
- ServiceNow
- Flow Designer
- Service Catalog
- Catalog Task
- No Node.js required

## Main Workflow
Standard Laptop Service Catalog → Request/Approval → Flow Designer → Create Catalog Task → Assignment Group: Hardware → Hardware configures laptop.

## Eight Project Phases
1. Brainstorming & Ideation
2. Requirement Analysis
3. Project Design
4. Project Planning
5. Project Development
6. Project Testing
7. Project Documentation
8. Project Demonstration

## Important Configuration
### Flow
- Flow Name: **Standard laptop task**
- Application: **Global**
- Run as: **System user**
- Trigger: **Service Catalog**
- Action: **Create Catalog Task**
- Requested Item Record: the request's Requested Item
- Short description: **Laptop need to Configured**
- Description: **Laptop need to Configured**
- Assignment group: **Hardware**
- Approval: **Approved**

### Service Catalog
- Maintain Item: **Standard Laptop**
- Process engine: remove remaining automations and add the created flow
- Flow assigned: **Standard Laptop Task**

## Demonstration
1. Open ServiceNow.
2. Open Service Catalog → Hardware → Standard Laptop.
3. Select Order Now.
4. Open the request number.
5. Open the Approvers section.
6. Approve the request.
7. Open the Requested Item.
8. Open Catalog Tasks.
9. Verify the updated task status, short description, and assigned group.

## Source
This repository is based on the supplied project document:
**Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer**
