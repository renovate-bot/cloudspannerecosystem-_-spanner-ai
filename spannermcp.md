# Overview

The Spanner remote MCP server standardizes how large language models (LLMs) and AI agents query and manage Spanner resources ([source](https://docs.cloud.google.com/spanner/docs/use-spanner-mcp)). It operates as a remote server on Google Cloud infrastructure, offering an HTTP endpoint for communication.

## Prerequisites for using with Antigravity

*   The Google Cloud CLI (`gcloud`) must be installed.
    *   You must be authenticated with `gcloud` (either `gcloud auth application-default login` or `gcloud auth login`).
*   A Google Cloud project with billing enabled and the **Spanner API** enabled ([source](https://docs.cloud.google.com/spanner/docs/use-spanner-mcp#before-you-begin)).
*   The following IAM roles are required :
    *   **MCP Tool User** (`roles/mcp.toolUser`): Required in addition to Spanner-specific IAM roles (such as `roles/spanner.admin`) to execute tool calls and perform operations via the Spanner remote MCP server.

## Documentation

For more detailed information, including available tools and security configurations like Model Armor, refer to the official documentation:
[Use the Spanner remote MCP server](https://docs.cloud.google.com/spanner/docs/use-spanner-mcp)
