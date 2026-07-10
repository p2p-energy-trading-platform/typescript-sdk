# GridX TypeScript SDK

Generated TypeScript protobuf SDK for the GridX - P2P Energy Trading Platform.

This SDK contains TypeScript protobuf types generated from the [`protobuf`](https://github.com/p2p-energy-trading-platform/protobuf) repository.

## Purpose

The TypeScript SDK is used by TypeScript services to share protobuf message and service contracts.

It can be used for:

- Kafka message encoding/decoding
- Connect/gRPC-style inter-service communication

## Generated Files

Do not manually edit files inside:

```text
src/gen/
```

These files are generated automatically from the protobuf contract repo.

## Install

Using GitHub tag dependency:

```bash
npm install github:p2p-energy-trading-platform/typescript-sdk#v0.2.0
```

## Usage

Import generated modules directly:

```ts
import { TestMoney } from "@p2p-energy-trading-platform/typescript-sdk/gen/gridx/test/v1/test_pb.js";

const money: TestMoney = {
  currencyCode: "LKR",
  units: BigInt(100),
  nanos: 0,
};
```

## Build

```bash
npm install
npm run build
```

## Versioning

This SDK follows the same version as the protobuf contract release.

Example:

```text
protobuf       v0.2.0
typescript-sdk v0.2.0
```


