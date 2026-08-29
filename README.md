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

## Ownership, licensing, and contributions

OpenAMRobot is a project initiated, operated, and controlled by **Botshare LTD** (Cyprus Company ID HE479056). Botshare LTD owns the transferable economic rights in original OpenAMRobot material created by or validly assigned to it. Third-party material remains subject to its respective ownership, licences, and notices.

Public distribution under this repository's applicable licence grants the permissions stated in that licence; it does not transfer ownership of underlying copyright, trademarks, patents, or other intellectual property.

Accepted external contributions require DCO sign-off and an applicable Individual or Corporate Contributor Agreement. See the organization [IP Policy](https://github.com/openAMRobot/.github/blob/main/IP_POLICY.md), [Contribution Guide](https://github.com/openAMRobot/.github/blob/main/CONTRIBUTING.md), and [Contributor Agreement Process](https://github.com/openAMRobot/.github/blob/main/CLA.md).
