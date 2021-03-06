# Segment-Branch

[![Version](https://img.shields.io/cocoapods/v/Segment-Branch.svg?style=flat)](http://cocoapods.org/pods/Segment-Branch)
[![License](https://img.shields.io/cocoapods/l/Segment-Branch.svg?style=flat)](http://cocoapods.org/pods/Segment-Branch)
[![Platform](https://img.shields.io/cocoapods/p/Segment-Branch.svg?style=flat)](http://cocoapods.org/pods/Segment-Branch)

## Usage

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

To install the Segment-Branch integration, simply add this line to your [CocoaPods](http://cocoapods.org) `Podfile`:

```ruby
pod "Segment-Branch"
```

## Usage

After adding the dependency, you must register the integration with our SDK.  To do this, import the Branch integration in your `AppDelegate`:

```
#import <Segment-Branch/BNCBranchIntegrationFactory.h>

```

And add the following lines:

```
NSString *const SEGMENT_WRITE_KEY = @" ... ";
SEGAnalyticsConfiguration *config = [SEGAnalyticsConfiguration configurationWithWriteKey:SEGMENT_WRITE_KEY];

[config use:[BNCBranchIntegrationFactory instance]];

[SEGAnalytics setupWithConfiguration:config];

```

## Author

Branch Metrics, support@branchmetrics.io

## License

Segment-Branch is available under the MIT license. See the LICENSE file for more info.
