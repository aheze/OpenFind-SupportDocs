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
- [Apple smoothie](https://aheze.github.io/FindInfo/Sample-Smoothies/Apple) (smoothies) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-Smoothies/Apple.md))
- [Blueberry smoothie](https://aheze.github.io/FindInfo/Sample-Smoothies/Blueberry) (smoothies) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-Smoothies/Blueberry.md))
- [Buy blue boba](https://aheze.github.io/FindInfo/Lists/BuyBlueBoba) (boba) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/BuyBlueBoba.md))
- [Buy cream boba](https://aheze.github.io/FindInfo/Lists/BuyCreamBoba) (boba) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/BuyCreamBoba.md))
- [Buy orange boba](https://aheze.github.io/FindInfo/Lists/BuyOrangeBoba) (boba) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Lists/BuyOrangeBoba.md))
- [How to cook pizza](https://aheze.github.io/FindInfo/Sample-FastFood/HowToCookPizza) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToCookPizza.md))
- [How to eat burritos](https://aheze.github.io/FindInfo/Sample-FastFood/HowToEatBurritos) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToEatBurritos.md))
- [How to eat grilled cheese](https://aheze.github.io/FindInfo/Sample-FastFood/HowToEatGrilledCheese) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToEatGrilledCheese.md))
- [How to eat nachos](https://aheze.github.io/FindInfo/Sample-FastFood/HowToEatNachos) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToEatNachos.md))
- [How to eat tacos](https://aheze.github.io/FindInfo/Sample-FastFood/HowToEatTacos) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToEatTacos.md))
- [How to make spaghetti](https://aheze.github.io/FindInfo/Sample-FastFood/HowToMakeSpaghetti) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToMakeSpaghetti.md))
- [How to prepare ramen](https://aheze.github.io/FindInfo/Sample-FastFood/HowToPrepareRamen) (fastFood) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-FastFood/HowToPrepareRamen.md))
- [Peach smoothie](https://aheze.github.io/FindInfo/Sample-Smoothies/Peach) (smoothies) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-Smoothies/Peach.md))
- [Plum smoothie](https://aheze.github.io/FindInfo/Sample-Smoothies/Plum) (smoothies) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-Smoothies/Plum.md))
- [Red berry smoothie](https://aheze.github.io/FindInfo/Sample-Smoothies/RedBerries) (smoothies) ([edit](https://github.com/aheze/FindInfo/edit/DataSource/Sample-Smoothies/RedBerries.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/aheze/FindInfo/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/aheze/FindInfo/edit/DataSource/_scripts/README.md). 
