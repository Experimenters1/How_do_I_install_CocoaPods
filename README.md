# How_do_I_install_CocoaPods
## How_do_I_install_CocoaPods?
#
### Install Homebrew on Mac : 

1. Install Homebrew:      https://brew.sh

2. Create .zshrc directory on terminal:  touch ~/.zshrc

3. Run this lines on terminal :    export PATH=/opt/homebrew/bin:$PATH
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
   
