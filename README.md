# SwiftUI-Pokedex
Create a Pokedex feature inside the BYU mobile app using SwiftUI.

Note: Use iOS 14 for the minimum target to take advantage of .onChange() and @StateObject
## Requirements:
- [ ] Create new branch off of dev
- [ ] Create Storyboard and UIHostingController to get to initial SwiftUI view
  - [ ] Create an initial SwiftUI view
    ````
    import SwiftUI
    
    struct SwiftUIView: View {
        var body: some View {
            Text("Hello, World!")
        }
    }
    ````
    - [ ] Create a storyboard and place a "HostingViewController" in it
    - [ ] Create a class like the one below that inherits from [UIHostingController](https://developer.apple.com/documentation/swiftui/uihostingcontroller)
     ````
    import Foundation
    import SwiftUI
    
    class UIHostingViewController: UIHostingController<SwiftUIView> {
        required init?(coder: NSCoder){
            super.init(coder: coder, rootView: SwiftUIView())
        }
        
    }
    ````
    - [ ] Assign the above class to the storyboard HostingViewController
- [ ] Display all Pokemon from Pokemon API in a [list](https://www.hackingwithswift.com/quick-start/swiftui/building-a-menu-using-list)
    - [ ] display a nagivation title
    - [ ] be able to search all pokemon by name
    - [ ] [each row must be clickable and use a navigation link to navigate to detailed view](https://www.hackingwithswift.com/articles/216/complete-guide-to-navigationview-in-swiftui)
    - [ ] use a list view model to handle searching, client calls, and other non-view operations 
    - [ ] [use the codable protocol on model objects with the json decoder](https://www.hackingwithswift.com/read/7/3/parsing-json-using-the-codable-protocol)
    - [ ] [use @Published property wrapper to publish changes in model object data to view](https://www.hackingwithswift.com/quick-start/swiftui/whats-the-difference-between-observedobject-state-and-environmentobject)
- [ ] Display an individual Pokemon in a detailed view
  - [ ] display the pokemons name
  - [ ] display the pokemon's image
  - [ ] display the pokemon's abilities
  - [ ] display the pokemon's types
  - [ ] use a detail view model to handle the client calls to get Pokemon details and other operations done in your detailed view

## Mentioned Resources:
 - [SwiftUI Lists](https://www.hackingwithswift.com/quick-start/swiftui/building-a-menu-using-list)

 - [NavigationView and NavigationLink](https://www.hackingwithswift.com/articles/216/complete-guide-to-navigationview-in-swiftui)

 - [Difference between @ObservedObject, @State, and @EnvironmentObject?](https://www.hackingwithswift.com/quick-start/swiftui/whats-the-difference-between-observedobject-state-and-environmentobject)

 - [Codable Protocol for deserializing json data](https://www.hackingwithswift.com/read/7/3/parsing-json-using-the-codable-protocol)

 - [How to run some code when state changes using onChange()](https://www.hackingwithswift.com/quick-start/swiftui/how-to-run-some-code-when-state-changes-using-onchange)

 - [What is the @Published property wrapper?](https://www.hackingwithswift.com/quick-start/swiftui/what-is-the-published-property-wrapper)

 - [UIHostingController Apple Documentation](https://developer.apple.com/documentation/swiftui/uihostingcontroller) 








