#UIImage` from the name of the item.
**The shopping items should be persisted between launches of the application.** On the first launch of the application, use the given shopping `itemNames` to create instances of the `ShoppingItem` model, and save them to a file using `FileManager`. To help you do this, read the following substeps: Use this snippet of names of images from the asset catalog to create instances of items in the `ShoppingList` model controller:

            let itemNames = ["Apple", "Grapes", "Milk", "Muffin", "Popcorn", "Soda", "Strawberries"]

 Use a `Bool` and the `UserDefaults` to make sure that new shopping items are initialized only once.

 Save the shopping list to a file using a `PropertyListEncoder` as the user makes changes.
 Test and verify that your app saves and loads changes to the shopping list (quit and relaunch the app).
A custom Collection View Controller that shows a list of shopping items. 
The Collection View Controller should be embedded in a navigation controller.
 A custom Collection View Controller Cell must display all the properties of the shopping item.
Upon selecting the custom cell, the item's `Bool` value should change from `true` to `false` or vice-versa. You can know when a cell has been selected by using the `didSelectItemAt` method in the `UICollectionViewDelegate` protocol
A bar button item on the Collection View Controller that performs a "Show" segue to a detail `UIViewController` subclass. This `UIViewController` should allow the user to fill in their name, address, and submit the order.
	1. The detail 
