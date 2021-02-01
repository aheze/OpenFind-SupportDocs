# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/aheze/SupportDocs#using-the-github-repo) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/aheze/FindInfo/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/aheze/FindInfo/DataSource/_data/supportdocs_datasource.json</a>

<details>
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/aheze/FindInfo/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/aheze/FindInfo/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://aheze.github.io/FindInfo/404) (SupportDocs Integrated File) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/FindInfo/404.md))
- [Caching photos](https://aheze.github.io/FindInfo/Photos/CachePhotos) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/CachePhotos.md))
- [Find from all photos](https://aheze.github.io/FindInfo/Photos/FindFromAllPhotos) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/FindFromAllPhotos.md))
- [Finding from Photos takes a long time](https://aheze.github.io/FindInfo/Photos/TakeLongTime) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/TakeLongTime.md))
- [Haptic Feedback](https://aheze.github.io/FindInfo/Settings/HapticFeedback) (settings) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Settings/HapticFeedback.md))
- [Hearting](https://aheze.github.io/FindInfo/Photos/Hearting) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/Hearting.md))
- [How do I delete a list?](https://aheze.github.io/FindInfo/Lists/DeleteList) (lists) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/DeleteList.md))
- [How to add a word](https://aheze.github.io/FindInfo/Lists/AddWord) (lists) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/AddWord.md))
- [How to delete a word](https://aheze.github.io/FindInfo/Lists/DeleteWord) (lists) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/DeleteWord.md))
- [Photos Controls](https://aheze.github.io/FindInfo/Photos/PhotosControls) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/PhotosControls.md))
- [Text Detected Indicator](https://aheze.github.io/FindInfo/Settings/TextDetection) (settings) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Settings/TextDetection.md))
- [Uncache Photos](https://aheze.github.io/FindInfo/Photos/Uncache) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/Uncache.md))
- [What are Lists?](https://aheze.github.io/FindInfo/Lists/WhatAreLists) (lists) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/WhatAreLists.md))
- [What is a Word to Find?](https://aheze.github.io/FindInfo/Lists/WordToFind) (lists) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/WordToFind.md))
- [What is the Cache?](https://aheze.github.io/FindInfo/Photos/WhatIsCache) (photos) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Photos/WhatIsCache.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/aheze/FindInfo/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/aheze/FindInfo/edit/DataSource/_scripts/README.md). 