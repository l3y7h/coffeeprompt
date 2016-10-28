# Coffee Prompt
A simple program that prompts the user to end the kind of coffee they want, the kind of milk they want (e.g. cream or steamed milk), and the kind of sweetener they want.

- - -

```javascript
var menu = [
					{
						drink: 'espresso',
						price: 3.45
					}, 
					{
						drink: 'mocha',
						price: 3.13
					},
					{
						drink: 'latte',
						price: 3.54
					},
					{
						condiment: 'milk',
						price: .65
					},
					{
						condiment: 'cream',
						price: .67
					}, 
					{
						condiment: 'sugar',
						price: .64
					}, 
					{
						codiment: 'vanilla',
						price: .64
					}
				 ];
		/**
		 * [total is the total cost of cup of coffee]
		 * @type {Number}
		 */
		var total = 0;
		// prompt user for what type of coffee
		var coffee = prompt("What type of coffee would like (mocha, latte, or espresso: ")
		// prompt user whether they would like to make it sweet
		var sweet = prompt("would you like to make it sweet?  (sugar or vanilla)");
		// ask user if they would like cream or milk
		var dairy = prompt("would you like to add cream or milk? (cream or milk)");
		// Loop through the array
		for (var i = 0; i < menu.length; i++) {
			// match users choice
			if(menu[i].drink === coffee) {
				//  compute a total price for the drink based on the various options the user has for drinks and condiments
				total += menu[i].price;
			}
			if(menu[i].condiment === sweet) {
				total += menu[i].price;
			}
			if(menu[i].condiment === dairy) {
				//  compute a total price for the drink based on the various options the user has for drinks and condiments
				total += menu[i].price;
			}
		}
```
