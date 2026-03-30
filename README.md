# marketplace-test

A test repository for experimenting with GitHub Copilot agent customization and plugin configurations.

## Overview

This workspace contains a plugin and agent definitions for an AI-native application security review system. It is used to validate agent discovery, invocation behavior, and marketplace plugin structure.

## Structure

```
plugins/
  reviews/
    plugin.json                          # Plugin manifest (v1.2.0)
    agents/
      working.agent.md                   # General-purpose test agent
      security-design/
        security-design-review.agent.md  # STRIDE threat modeling & architecture review agent
```

## Plugins

### reviews

Enterprise-grade AI-native application security scanning, validation, and remediation.

- **Version:** 1.2.0
- **License:** Apache-2.0
- **Keywords:** security, vulnerability, management, enterprise, scanning, validation, remediation

## Agents

### Working Test Agent

A minimal agent used to verify that agent files are discovered and invoked correctly. Supports `read` and `search` tools only.

### design-review

A senior application security architect agent that performs STRIDE threat modeling and architecture security reviews. It auto-detects repo type, evaluates design principles and trust boundaries, and delivers risk-prioritized remediation recommendations.

**Supported tools:** `read`, `search`, `web`, `edit`
