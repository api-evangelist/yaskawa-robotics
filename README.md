# yaskawa-robotics

Yaskawa / Motoman — industrial robotics, AC servo motors, drives, and motion control.

Yaskawa Electric Corporation (Kitakyushu, Japan) is the world's largest manufacturer of AC servo motors and motion controllers, and one of the most established industrial robotics vendors through its Motoman brand. This api-evangelist profile catalogs Yaskawa's developer-facing surface across four business segments: **Motion Control** (Sigma-X servo motors and SERVOPACK amplifiers), **AC Drives / Inverters** (GA800, U1000, low- and medium-voltage VFDs), **Robotics** (Motoman articulated, SCARA, delta, mini, and collaborative robots on DX200, YRC1000, and YRC1000micro controllers), and **Systems Engineering**.

## Developer Surface

Yaskawa's developer presence is **SDK- and protocol-driven**, not HTTP/REST. There are no public OpenAPI specifications, so this profile intentionally omits a generated `openapi/` directory. The catalog instead points to:

- **[Yaskawa Motoman Developer Portal](https://developer.motoman.com/en/home)** — the central hub for SDK docs, how-tos, and YIP packages.
- **[Yaskawa-Global on GitHub](https://github.com/Yaskawa-Global)** — official open-source repositories.
- **[YMConnect](https://github.com/Yaskawa-Global/YMConnect)** — modern PC-side communication library for controlling Motoman robots from custom applications (C++ 17 and C#).
- **[MotoROS2](https://github.com/Yaskawa-Global/motoros2)** — a native ROS 2 (rcl, rclc, micro-ROS) node running on MotoPlus-compatible controllers; supports ROS 2 Foxy, Galactic, Humble, and Jazzy, up to 8 motion groups, ~100 Hz control.
- **MotoPlus SDK** — on-controller C development for deterministic timing, multi-tasking communication, position/motion data, variables, I/O, jobs, and alarm/error handling.
- **[MotoCom SDK](https://www.motoman.com/en-us/products/software/development/motocom-sdk)** — legacy Windows SDK for status monitoring, I/O exchange, and variable management.
- **[SmartPendantSDK](https://github.com/Yaskawa-Global/SmartPendantSDK)** — Java SDK for extending the Smart Pendant teach interface.
- **[Smart Packager](https://developer.motoman.com/en/yip/smart-packager)** — tooling for building YIP (Yaskawa Innovation Plus) extension packages.

## Profile Contents

- [`apis.yml`](./apis.yml) — APIs.json 0.20 catalog entry for Yaskawa / Motoman.

## Related

- [api-evangelist/figure-robotics](https://github.com/api-evangelist/figure-robotics) — Figure (humanoid robotics).
