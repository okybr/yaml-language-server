# Fork of YAML Language Server based on JSON-Schema Draft 04

This is a fork of [yaml-language-server](https://github.com/redhat-developer/yaml-language-server) which uses [ajv-draft-04](https://github.com/ajv-validator/ajv-draft-04) and is thus based on JSON-Schema Draft 04 (instead of JSON-Schema Draft 07).
The difference is [this single commit](https://github.com/okybr/yaml-language-server/commit/455d452f66c700a3101f87b3970f882c3967e986).

In particular, this fork supports [the official schema-definition OpenAPI version 3.0](https://github.com/OAI/OpenAPI-Specification/blob/main/schemas/v3.0/schema.json) (which is based on Draft 04) and is a work-around for these issues:

- https://github.com/OAI/OpenAPI-Specification/issues/2969
- https://github.com/redhat-developer/yaml-language-server/issues/752

## Why is this a fork?

It would be better to change upstream yaml-language-server so that you can choose a draft version.
I made this a fork just because of I'm too lazy to implement the better, flexible solution.
