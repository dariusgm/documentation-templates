# project-name

This README.md is inspired by this [template](https://github.com/dariusgm/documentation-templates).

You may not need every aspect of the templates, but they give you an idea what *can* be
documented in your projects.

    Good documentation reflect any granularity of your project.

"But I don't need everything" - that is totally fine. Just skip it and leave
the block blank. Maybe in the future you will add documentation their.

For more general information, see [general](general.md)


# Team Documentation


## Snippets

### Example 1
This snippets extract a list of directories.

```bash
ls -dl /home/darius/*/ | awk -F'[[:space:]]' '{print $NF}' | bash
```

## Code Documentation

Please apply general best practice for software development.

## Applications

### ls
#### Input
##### path String
`path` is the path that you want to list the content of

#### Output Array[String]
List of directories

### com.example.java.Main
#### Input
##### number integer
`number` is the number to process.

#### Output Float
heavy number computations

## Installation

For general installation guide, see the [general](general.md) documentation.
For this project you need java 11 that be installed via homebrew:
```bash
brew install java@11
```

## Local Configuration
### Environment variables
set DEBUG=1 to enable debugging.

## Secrets

The credentials for accessing the servers can be found in the
[credentials repository](https://www.murawski.blog)

## Access Test/Staging/Production

### VPN Settings
* IP / Host
* Password
* Cert
* CA


### SSH Key
The ssh key can be found in `Secrets`

### Jumphost
You can access the production server via the Jumphost on 127.0.0.1.
```bash
ssh -i key.pem -N -L 8156:127.0.0.1:8156 root@example.com
```

## Deployment

How deployment is triggered?

## Tests

How tests need to be executed?

## FAQ

Some FAQ for the application.


# Company Documentation

## Requirements
### Functional Requirements
* What business problem should be solved?

### Non-Functional Requirements
Try to convert them to functional requirements where possible.
For example, instead of **fast**, write: "The application needs to answer in 10ms"

## Stakeholders

Who are the stakeholders and how to reach them?

## Data Privacy

What kind of data is collected or processed and what data privacy
regularization need to be taken into account?

## Data Schema
### Columns and Types
### Distribution

## Tool Distribution
What Frameworks are used?

## Architecture / Design
* Why this architecture was selected?
* What design where discusses but not selected and why?

## Monitoring
* What monitoring is applied for the service and what metrics are most important?

## Errors handling
The service is returning some amount of errors. What to do in this case?

## Service stop
The service stopped working at night (for example terminated). What to do in this case?

## Infrastructure provisioning
How is responsible for provisioning / updating the underlying hardware?

## Security
How is responsible for security of the application and the operating system with their dependencies?

## Big Picture
What step is done before and after this applications finish? How is the data handed over to the next team?


# external Companies / Partners

This section now describe information that are relevant for external Partners.

## Public API

In case you are providing a public api you can document a lot!

### Access to the api user
How to get access as user?

### Testing
Where to send test calls?

### Swagger
Do you provide a public swagger documentation for the users?

### Data model
How does the data model look like?

#### Input data model
* Keys and values with their types.

#### Output data model
* Keys and values with their types.

#### error data model
What is returned in case of errors? What errors are can be returned by the api?


## Manual / Tutorial
Description of how to use the software in case you have some frontend.
How about a video that shows the usage of the software?

## Artifacts
When you provide libraries or any other artifacts that can be included by the user, describe how to do it. Ideally create a minimal repository with an example.

# Final Words
Documentation have to be taken care. Update it as often as possible.
