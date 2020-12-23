# Backend-test

- Create an endpoint that receives and persist a product with the following attributes: name, price, quantity, type and tax_formula
- We have two possible types: national product and international product
- For the tax_formula, you should parse a string and we need to accept +, -, * and / as operators
  - Examples of formula: price * quantity + 10, (price * 0.10)/quantity
- For international products we should sum 50% of product in the value that we calculated after running the tax_formula
  - For instance, you have a product with price as $1000, after you run the tax_formula you calculate that the tax for the product is $100. For national products the tax will be $100, for international products the tax will be $100 + $500 = $600.
- Create an architecture that is easy to add new types of products. We currently have only national and international products. What if we need to add 10 more types?
