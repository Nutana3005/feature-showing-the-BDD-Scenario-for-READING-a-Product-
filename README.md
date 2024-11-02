# feature-showing-the-BDD-Scenario-for-READING-a-Product-
Scenario: Reading a product
  Given the following products
    | name   | category | available |
    | ToyCar | Toys     | true      |
  When I retrieve the product by name "ToyCar"
  Then I should see the product with name "ToyCar" and category "Toys"
