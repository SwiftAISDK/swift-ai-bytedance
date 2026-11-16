<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-bytedance 1.1.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-bytedance.git", from: "1.1.0")
```

Products: `SwiftAIByteDance`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# ByteDance (BytePlus ModelArk) for Swift

`SwiftAIByteDance` adds ByteDance (BytePlus ModelArk) to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/bytedance` and supports video generation.

Provider guide with models, options, streaming and errors:

- [ByteDance (BytePlus ModelArk)](https://swiftaisdk.github.io/SwiftAISDK/providers/bytedance/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIByteDance` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIByteDance

let provider = try AIProviders.byteDance(configuration: ByteDanceProviderSettings())
```

By default the provider reads `ARK_API_KEY` from the environment; values set in `ByteDanceProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-bytedance` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
