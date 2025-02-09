# Namedata Project

**User Friendly Semantic Model Naming Convention for Power BI**

This guide provides a set of naming conventions to ensure clarity, consistency, and ease of use within Power BI semantic models. The rules apply to all model objects, including tables, columns, measures, and other technical elements.

---

### 1. Readable

**Rule Definition:**  
- Object names use a CamelCase style for clarity but allow spaces between words. This applies to tables, columns, and measures in Power BI.

**Rationalisation:**  
> **Why?**  
> Allowing spaces improves readability in Power BI reports and dashboards, making it easier for report authors to quickly understand and work with the data.

**Antipatterns:**  
- Using compact names without spaces (e.g., "CustomerName" instead of "Customer Name").  
- Overly abbreviated or merged styles that reduce clarity.

---

### 2. Consistent

**Rule Definition:**  
- The naming standard applies to all objects in the semantic model—including visible tables, hidden columns, and technical measures—to ensure uniformity across the model. For example, consistently using "Customer Name" or simply "Customer" throughout the model maintains standardization.

**Rationalisation:**  
> **Why?**  
> A uniform naming approach helps both business users and developers navigate the model. Adopting terms from the company’s common dictionary ensures that the language is familiar and consistent across all Power BI reports.

**Antipatterns:**  
- Mixing different naming styles (e.g., "customer_name" in one table and "Customer Name" in another).  
- Ignoring technical or hidden objects when applying naming conventions.

---

### 3. Simplified

**Rule Definition:**  
- When context allows, unnecessary words should be removed. For example, "Company Name" can be shortened to "Company" if the meaning is clear within the model.

**Rationalisation:**  
> **Why?**  
> Simplifying names reduces clutter in the Power BI model, making it easier for users to identify key concepts quickly and reducing the chance of misinterpretation.

**Antipatterns:**  
- Adding redundant words that add no extra value (e.g., "Customer Full Name" when "Customer" is sufficient).  
- Overcomplicating object names with extra, unnecessary descriptors.

---

### 4. Business Keys

**Rule Definition:**  
- Business key names should always end with "Id". For example, use "Customer Id" to clearly indicate a unique identifier within tables and relationships.

**Rationalisation:**  
> **Why?**  
> Appending "Id" to business keys signals that the object is a unique identifier, aiding in linking tables and reducing ambiguity. This consistency is crucial for both model integrity and ease of use by report developers.

**Antipatterns:**  
- Omitting the "Id" suffix (e.g., using "Customer" instead of "Customer Id").  
- Using inconsistent suffixes like "Key" or "Code".  
- Using "ID" (all uppercase) instead of "Id", since "Id" is the accepted shorthand for Identity.

---

### 5. Role-Playing Attributes

**Rule Definition:**  
- Role-playing objects (such as date fields used in multiple contexts) should include the role in parentheses after the main name. For instance, "Date (Order)" or "Date (Delivery)" clarifies the attribute's specific use. This rule applies to all objects in the model, including technical ones.

**Rationalisation:**  
> **Why?**  
> Specifying the role in parentheses helps both business and technical users understand the context in which an attribute is used, particularly when the same field serves multiple purposes within Power BI.

**Antipatterns:**  
- Not indicating the role for objects that serve multiple purposes.  
- Using inconsistent or unclear formatting for role indicators (e.g., "OrderDate" instead of "Date (Order)").







# Entities

# Mapping Tables

# Dimentions and attributes

## Surrogate keys
## Date is not a conformed dimention
## Dummy records

## Degenerate dimentions

## Junk dimention (do not use)

# Facts

Not visible to end users
Star, conctelation, snowflake.

## Bridge tables

### Row-level-secutity

## Measures (aggregatables)

## Many-to-many relationships

## Aggregated tables or composite models

Just a tool. Do not use before performance is a problem.

# Technics
## Avoiding distinct count in DAX
## Calculation groups

