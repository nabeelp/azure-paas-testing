# Azure PaaS Testing
Performance testing of various Azure PaaS services, to determine and document the impact on performance of varied configurations and architectures

# Guiding Principles

The principles adhered to in this effort, designed to ensure we focus on testing performance variations on the most common scenarios.

1. We will always use the latest released versions of coding languages, where applicable.
2. Focus on testing variations in service configuration and not on coding variations, by keeping coding to the minimal required for the test. An exception is where the coding variation has a material impact on the performance of the service. For example, using different methods of binding in Functions is acceptable, while optimising business logic is not.

# Structure

At a high level, the tests are organised according to the following structure:

- [Services](/services/) - tests that relate to single Azure services only, e.g. Web Apps, Logic Apps, API Management, etc.
- [Scenarios](/scenarios/) - tests that are composed of 2 or more Azure services, and are intended to represent common service combinations, e.g. Web App + SQL, APIM + Function App, etc.

Within [Services](/services/) there be multiple variations, based on the configuration options that have an impact on the performance of that service.  For example, the Logic Apps service tests will be structured to reflect differences in the Consumption and Standard tiers, and the different hosting models for each of these tiers. Within these there may be multiple test cases to reflect different load testing profiles and performance-related configuration settings.

Test within [Scenarios](/scenarios/) will re-use the resources created within the [Services](/services/) folder to create a composite test case for a specific scenario.

# Current Status

- Initial structure defined

# Plans

- Create Logic Apps consumption HTTP trigger test

# Contributing

TODO: Provide contribution guidelines