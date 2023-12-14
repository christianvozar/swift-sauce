
# SAUCE Swift Package

## Overview

The SAUCE Swift Package provides a set of tools for handling SAUCE (Standard Architecture for Universal Comment Extensions) records in files. SAUCE comes from the DOS era for attaching metadata or comments to files, predominantly used in ANSI art files. This package enables Swift applications to read, write, and manipulate SAUCE data, making it easier to work with this kind of metadata in a Swift-based environment.

### Why Use SAUCE Swift Package?

- **Standardized Metadata Management**: Easily handle standardized metadata in ANSI art files and other supported formats.
- **Read and Write Capability**: Read existing SAUCE data from files and write new or updated SAUCE records.
- **Swift Integration**: Seamlessly integrates with Swift projects, providing a native Swift interface for SAUCE operations.
- **Open Source**: Modify and adapt the package to fit specific needs or contribute improvements back to the community.

## Installation

To use the SAUCE Swift Package in your project, simply clone the repository or download the source files into your project directory.

```
git clone https://github.com/christianvozar/sauce-swift-package.git
```

## Usage

### Reading SAUCE Data

To read SAUCE data from a file:

```swift
import Foundation

if let sauce = SAUCEReader.readSAUCE(fromFileAtPath: "path/to/your/file") {
    print("SAUCE Data: \(sauce)")
} else {
    print("No SAUCE data found or failed to read the file.")
}
```

### Writing SAUCE Data

To write SAUCE data to a file:

```swift
import Foundation

let sauce = SAUCE() // Populate your SAUCE data
SAUCEWriter.writeSAUCE(sauce, toFileAtPath: "path/to/your/file")
```

## Contributing

Contributions to the SAUCE Swift Package are welcome. Please feel free to submit pull requests, report bugs, or suggest features.

## License

This SAUCE Swift Package is open source and available under the [MIT License](LICENSE).
