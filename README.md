js file:

// global variables
let cart = [];
let cartTotal = 0;

on addToCart click:
// push object to cart list 
cart.push( {name: ${name of print}, price: "$15"} );
// increment nav header by icon (${cart.length})
$('#headerID').text(`cart ($(cart.length))`);
// adjust cartTotal
cartTotal += 15;

on removeFromCart click:
// remove item from cart list
 // how to remove that specific object... search for matching name? in keys, iterate through
 // need to use let i = o, cart.splice(i, 1); when found at index i...
//decrememnt nav header by icon
$('#headerID').text(`cart ($(cart.length))`);
// adjust cartTotal
cartTotal -= 15;

in index/prints html:
make cart dropdown on icon hover (hide otherwise)
x botton to remove item from cart
display cart array
display total
checkout button links to /checkout.html

in checkout html:
option to remove from cart => remove from array, decremements nav header, decremements total
