# OpenAMRobot Communication

Communication protocols, APIs, middleware bridges, transport layers, and interoperability definitions for the OpenAMRobot ecosystem.

## Repository Status

Current maturity level: Experimental

## Purpose

This repository defines communication patterns and integration contracts between OpenAMRobot subsystems, including:

- UI to robot communication
- ROS 2 bridge definitions
- REST API conventions
- WebSocket event streams
- MQTT topics
- serial communication conventions
- cloud or fleet-management bridges
- telemetry schemas
- command schemas
- interoperability documentation

## Repository Structure

```text
openamrobot-comm/
├── protocols/
│   ├── rest/
│   ├── websocket/
│   ├── mqtt/
│   ├── serial/
│   └── ros2_bridge/
│
├── middleware/
│   ├── ros2/
│   ├── ui_bridge/
│   ├── cloud_bridge/
│   └── fleet_management/
│
├── schemas/
│   ├── json/
│   └── yaml/
│
├── docs/
├── examples/
├── tests/
└── tools/
```

## Repository Boundaries

This repository defines communication contracts and middleware patterns.

ROS 2 package implementations belong in:

```text
openamr-platform-sw
```

Embedded firmware implementations belong in:

```text
openamr-platform-fw
```

Shared ROS 2 messages, services, and actions belong in:

```text
openamrobot-interfaces
```

User interface implementation belongs in:

```text
openamrobot-ui
```

## Design Principles

Communication interfaces should be:

- clearly documented
- versioned
- secure by design
- transport-aware
- reusable
- testable
- compatible with simulation and real hardware
- suitable for future fleet and cloud integration

## Future Scope

Planned future work may include:

- REST API specification
- WebSocket telemetry schema
- MQTT topic conventions
- serial protocol definitions
- UI-to-ROS bridge documentation
- fleet management communication contracts
- security and authentication guidelines

## License

MIT License.