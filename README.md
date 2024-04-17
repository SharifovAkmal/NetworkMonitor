# NetworkMonitor

NetworkMonitor is a lightweight Swift class that provides functionality to monitor network connectivity and determine the current connection type in iOS applications.

## Overview

Network connectivity is crucial for many mobile applications, especially those that rely on real-time data or communication with remote servers. NetworkMonitor simplifies the process of monitoring network status changes and provides information about the current network connection type.

## Features

- **Network Monitoring**: Constantly monitors network connectivity in the background.
- **Connection Type Detection**: Determines whether the device is connected via Wi-Fi, cellular data, Ethernet, or unknown connection types.
- **Simple Integration**: Easy to integrate into any iOS application.

## Usage

To use NetworkMonitor in your iOS application:

1. Add the `NetworkMonitor.swift` file to your Xcode project.
2. Initialize an instance of `NetworkMonitor` in your code.
3. Start monitoring network connectivity by calling `startMonitoring()`.
4. Stop monitoring when no longer needed by calling `stopMonitoring()`.

```swift
// Example Usage:

import UIKit

class ViewController: UIViewController {
    private let networkMonitor = NetworkMonitor.shared
    
    override func viewDidLoad() {
        super.viewDidLoad()
        
        // Start monitoring network connectivity
        networkMonitor.startMonitoring()
    }
    
    override func viewWillDisappear(_ animated: Bool) {
        super.viewWillDisappear(animated)
        
        // Stop monitoring network connectivity
        networkMonitor.stopMonitoring()
    }
}
```

## REQUIREMENTS

- iOS 10.0+
- Swift 5.0+


## Installation

Simply copy the `NetworkMonitor.swift` file into your Xcode project.


## LICENSE

This code is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
