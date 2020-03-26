# Shipping Tax Class

In most setups, shipping tax class is inherited from the item being shipped, e.g., Shipping a reduced rate item such as baby clothes would also use a reduced rate. If this is not the case in your jurisdiction, choose a different tax class.

In the case of multiple tax rates in the order, the shipping tax will be applied as follows:

* If you have a product with the `Standard` rate in the order, it will be used for the shipping regardless if this rate is high or low;
* If you don’t have a product with the `Standard` rate in the order, then the first rate found in the `Additional tax class` section will be used for shipping.

The goal is to make sure that your highest rate is listed the first in the `Additional tax class` section if you don’t use the `Standard` class and if you need the highest tax rate to apply to shipping, for example.

### Here is a setup to showcase it visually:

The `Standard` class is there by default but `Tax A`, `Tax B`, `Tax C` should be created for each tax class respectively. Note that it is not possible to delete the `Standard` tax rate but you can leave it empty and it will be ignored:

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/1.jpg?w=471)

#### `Standard` rate is empty:

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/2.png?w=550)

#### `Tax A` \(24%\) – the highest rate listed the first:

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/3.png?w=550)

#### `Tax B` \(14%\):

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/4.png?w=550)

#### `Tax C` \(10%\):

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/5.png?w=550)

As a result, the highest tax rate gets applied to the shipping in the order with multiple tax rates assigned to products:

![](https://docs.woocommerce.com/wp-content/uploads/2013/02/6.jpg?w=550)

