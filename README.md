# How_do_I_install_CocoaPods
## How_do_I_install_CocoaPods?
[How_do_I_install_CocoaPods?](https://stackoverflow.com/questions/20755044/how-do-i-install-cocoapods) <br><br>
#
### Install Homebrew on Mac : 

1. Install Homebrew:      https://brew.sh

2. Create .zshrc directory on terminal:  touch ~/.zshrc

3. Run this lines on terminal :    export PATH=/opt/homebrew/bin:$PATH <br>
         source ~/.zshrc

4. Check If Homebrew is available:  brew help

5. Install Cocoapods, run on terminal:   brew install cocoapods

6. Now, Cocoapods is available

Install pods in your project:

1. Open your project folder at terminal.

2. Run on terminal “pod init” to create podfile.

3. Open pod file and insert any pod, for example, “PryntTrimmerView” : pod "PryntTrimmerView".

4. Run on terminal “pod install” to install pods.

5. Now, you can import pods into your project.

#
### Package.swift
Tệp **Package.swift** thường được sử dụng trong các dự án Swift Package Manager (SPM). SPM là một công cụ được tích hợp sẵn trong Xcode để quản lý và cài đặt các gói thư viện Swift.

Nếu dự án của bạn sử dụng SPM và có một tệp **Package.swift**, bạn sẽ tìm thấy nó ở thư mục gốc của dự án của bạn. Thường, nó sẽ nằm cùng cấp với tệp ***.xcodeproj** hoặc ***.xcworkspace.**

Để tạo một tệp **Package.swift** mới trong một dự án, bạn có thể sử dụng lệnh sau trong Terminal:

<div class="code-snippet">
  <pre>
    <code>
       swift package init      
    </code>
  </pre>
  <button class="copy-button" data-clipboard-target=".code-snippet"></button>
</div> <br>

Lệnh này sẽ tạo một tệp **Package.swift** trong thư mục hiện tại, và bạn có thể chỉnh sửa nó để thêm các phụ thuộc và cài đặt cho dự án SPM của mình.

#
Để thêm phụ thuộc vào tệp **Package.swift**, bạn có thể thực hiện các bước sau:

1.Mở tệp **Package.swift** trong trình soạn thảo văn bản của bạn.

2.Tìm phần **"dependencies"** trong tệp **Package.swift.** Nếu nó không tồn tại, hãy thêm nó vào bên trong Package:
<div class="code-snippet">
  <pre>
    <code>
       dependencies: [
    // ... các phụ thuộc hiện có của bạn
]      
    </code>
  </pre>
  <button class="copy-button" data-clipboard-target=".code-snippet"></button>
</div> <br>


Thêm phụ thuộc của bạn vào mảng **dependencies.** Đối với PryntTrimmerView, bạn đã cung cấp URL của kho lưu trữ GitHub và yêu cầu phiên bản từ 4.0.1 trở lên, bạn có thể thêm nó như sau:
<div class="code-snippet">
  <pre>
    <code>
dependencies: [
    .package(url: "https://github.com/HHK1/PryntTrimmerView.git", .upToNextMajor(from: "4.0.1"))
]
    </code>
  </pre>
  <button class="copy-button" data-clipboard-target=".code-snippet"></button>
</div> <br>

Sau khi đã thêm phụ thuộc, tệp **Package.swift** của bạn có thể trông giống như sau:

```swift

// swift-tools-version:5.5
// The swift-tools-version declares the minimum version of Swift required to build this package.

import PackageDescription

let package = Package(
    name: "YourPackageName",
    products: [
        // Define your products here, for example:
        // .library(name: "MyLibrary", targets: ["MyLibrary"]),
    ],
    dependencies: [
        // Dependencies declare other packages that this package depends on.
        .package(url: "https://github.com/HHK1/PryntTrimmerView.git", .upToNextMajor(from: "4.0.1"))
    ],
    targets: [
        // Targets are the basic building blocks of a package. A target can define a module or a test suite.
        // Targets can depend on other targets in this package, and on products in packages which this package depends on.
        // .target(name: "MyLibrary", dependencies: []),
        // .testTarget(name: "MyLibraryTests", dependencies: ["MyLibrary"]),
    ]
)

```

Lưu tệp **Package.swift**.

Sau đó, bạn có thể sử dụng Swift Package Manager để cập nhật phụ thuộc bằng lệnh sau trong Terminal:
<div class="code-snippet">
  <pre>
    <code>
         swift package update
    </code>
  </pre>
  <button class="copy-button" data-clipboard-target=".code-snippet"></button>
</div> <br>





