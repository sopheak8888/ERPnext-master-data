To set up **Pricing and Discounts** in **ERPNext** for **Inventory Management** or **POS**, you need to configure Price Lists, Item Pricing, and Discount Rules. Here’s a step-by-step guide to help you set it up:

### 1. **Create or Update a Price List**

- Go to **Selling > Items and Pricing > Price List**.
- Create a new Price List or edit an existing one (e.g., "Retail Price List").
- You can have multiple Price Lists, such as **Retail Price** or **Wholesale Price**.

### 2. **Set Item Prices**

- Go to **Selling > Items and Pricing > Item Price**.
- Click on **New** and fill in the details:
  - **Item**: Select the item for which you want to set the price.
  - **Price List**: Choose the Price List (e.g., "Retail Price List").
  - **Rate**: Set the price of the item.
- You can set different prices for the same item under different Price Lists (e.g., retail vs. wholesale prices).

### 3. **Configure Pricing Rules**

Pricing Rules allow you to apply discounts or price adjustments automatically.

- Go to **Selling > Items and Pricing > Pricing Rule**.
- Click on **New** and fill in the details:
  - **Apply On**: Choose whether this applies to a **Price List**, **Item Group**, **Customer Group**, or **Territory**.
  - **Item Code**: Specify the item(s) or **Item Group**.
  - **Min Qty**: Set a minimum quantity for this rule to apply (if applicable).
  - **Applicable For**: Specify if it applies to **Selling**, **Buying**, or **POS**.
  - **Price List**: Select which Price List the rule applies to.
  - **Rate or Discount**: Choose if this rule is based on a fixed rate or a percentage discount. You can enter either a discount percentage or a new rate.

**Example**:

- A 10% discount for a specific product when purchased in a quantity of 5 or more.
- A different price for wholesale customers based on their **Customer Group**.

### 4. **Set Discounts on Items or POS**

- **For POS**: Ensure the **Price List** and **Pricing Rules** are properly configured, as the system will automatically apply the right price based on the rules.
- In **POS** settings, you can allow manual discounts:
  - Go to **POS Profile** and enable settings like **Allow User to Edit Discount** if you want to provide flexibility to the cashier.

### 5. **Customer-Specific Pricing**

- If you want to set up specific pricing for certain customers, you can do so under the **Customer** form.
- You can assign a default Price List to specific customers or set up **Pricing Rules** for customer groups like **VIP** or **Wholesale** customers.

### 6. **Check the Setup in POS/Inventory**

- After setting up your Price Lists, Item Prices, and Pricing Rules, make a few test transactions in the **POS** or inventory system to ensure that the pricing and discounts are applied correctly.

### Additional Tips:

- **Currency Adjustments**: If you deal with multiple currencies, set up different Price Lists for each currency.
- **POS Profile**: Ensure that your POS profile has the correct Price List selected under **Selling > POS > POS Profile**.