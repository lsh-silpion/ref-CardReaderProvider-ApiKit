# CardReaderProvider-ApiKit

(Smart)CardReader protocols for interacting with [HealthCardAccessKit](http://www.github.com/gematik/HealthCardAccessKit).

## Getting Started

CardReaderProvider-ApiKit requires Swift 5.1.

### Setup for integration:

-   **Carthage:** Put this in your `Cartfile`:

        github "gematik/ref-CardReaderProvider-ApiKit" ~> 1.0

### Setup for development

You will need [Bundler](https://bundler.io/), [XcodeGen](https://github.com/yonaskolb/XcodeGen)
and [fastlane](https://fastlane.tools) to conveniently use the established development environment.

1.  Update ruby gems necessary for build commands

        $ bundle install --path vendor/gems

2.  Checkout (and build) dependencies and generate the xcodeproject

        $ bundle exec fastlane setup

3.  Build the project

        $ bundle exec fastlane build_all [build_mac, build_ios]
