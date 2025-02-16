1.
As a member of the public,
So I can order a bagel before work,
I'd like to add a specific type of bagel to my basket.
| Classes | Methods                     | Scenario                     | Outputs          |
|---------|-----------------------------|------------------------------|------------------|
|`Basket` | `Add(string bagel)`         | add bagel to basket          | Boolean          |
|`Item`   |                             |                              |                  |

2.
As a member of the public,
So I can change my order,
I'd like to remove a bagel from my basket.
| Classes | Methods                     | Scenario                     | Outputs            |
|---------|-----------------------------|------------------------------|--------------------|
|`Basket` | `Remove(string bagel)`      | remove bagel from basket     | Boolean            |
|`Item`   |                             |                              |                    |

3.
As a member of the public,
So that I can not overfill my small bagel basket
I'd like to know when my basket is full when I try adding an item beyond my basket capacity.
| Classes | Methods                            | Scenario                                   | Outputs        |
|---------|------------------------------------|--------------------------------------------|----------------|
|`Basket` | `FullBasket(List<Item> items`      | check if basket full before adding item    | Boolean        |
|`Item`   |                                    |                                            |                |

4.
As a Bob's Bagels manager,
So that I can expand my business,
I�d like to change the capacity of baskets.
| Classes | Methods                       | Scenario                                    | Outputs        |
|---------|-------------------------------|---------------------------------------------|----------------|
|`Basket` | `BasketCapacity(int newCap)`  | change capacity of basket to provided int   | Int            |
|`Item`   |                               |                                             |                |

5.
As a member of the public
So that I can maintain my sanity
I'd like to know if I try to remove an item that doesn't exist in my basket.
| Classes | Methods              | Scenario                                       | Outputs        |
|---------|----------------------|------------------------------------------------|----------------|
|`Basket` | `SchrodingersBagel`  | check if item exists in basket before removing | Boolean        |
|`Item`   |                      |                                                |                |

6.
As a customer,
So I know how much money I need,
I'd like to know the total cost of items in my basket.
| Classes | Methods              | Scenario                               | Outputs        |
|---------|----------------------|----------------------------------------|----------------|
|`Basket` | `Total(Item item)`   | list total cost of items in my basket  | Double         |
|`Item`   |                      |                                        |                |

7.
As a customer,
So I know what the damage will be,
I'd like to know the cost of a bagel before I add it to my basket.
| Classes | Methods              | Scenario                   | Outputs      |
|---------|----------------------|----------------------------|--------------|
|`Basket` | `Price(Item item)`   | list cost of chosen bagel  | Double       |
|`Item`   |                      |                            |              |

8.
As a customer,
So I can shake things up a bit,
I'd like to be able to choose fillings for my bagel.
| Classes | Methods                    | Scenario                          | Outputs        |
|---------|----------------------------|-----------------------------------|----------------|
|`Basket` | `changeFilling(Item item)` | change filling for chosen bagel   | String         |
|`Item`   |                            |                                   |                |

9.
As a customer,
So I don't over-spend,
I'd like to know the cost of each filling before I add it to my bagel order.
| Classes | Methods              | Scenario               | Outputs             |
|---------|----------------------|------------------------|---------------------|
|`Basket` | `Price(Item item)`   | list price of filling  | Double              |
|`Item`   |                      |                        |                     |

10.
As the manager,
So we don't get any weird requests,
I want customers to only be able to order things that we stock in our inventory.
| Classes | Methods                | Scenario                          | Outputs        |
|---------|------------------------|-----------------------------------|----------------|
|`Basket` | `InInventory(basket)`  | check if order items are in stock | Boolean        |
|`Item`   |                        |                                   |                |