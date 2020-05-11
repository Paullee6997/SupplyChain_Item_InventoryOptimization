# SupplyChain_Item_InventoryOptimization

This project was done for the supply chain management team at Saint Peter's Health Partners and Trinity Health. The primary focus of the project was based on the optimization of product inventory levels for their regional warehouse which supports up to 30 hospitals, geriatric centers and health facilities in the New York Capital region. With permission to post my analysis work online, I dive into the inventory optimization techniques used.

There is exploratory data analysis that was conducted at item level, but this was exlcuded from the notebook as not to divulge private company information. The general approach taken was to determine categories or groupings of items in the regional warehouse that share similar properties. In order to determine these groupings we must first discuss velocity, criticality and the ABC-VED analysis.

Velocity is the speed at which items move out of the warehouse in orders received from hospitals and geriatric centers. In the analysis, I define velocity to be based on overall yearly consumption of items which is reflective of item demand. The demand was adjusted to not include the unusual behaviors exherted on the healthcare system due to the Covid-19 emergency. 

Criticality has been defined by SPHP as three tiers ranging from 1-3 with 1 being less critical and 3 being very critical. Originally defined to be based on item family groups which is reflective of department usage of item, criticality must be quantified in future analysis.

Using Velocity and Criticality, ABC-VED analysis is conducted where three categories for items are created with each category containing items based on cutoffs which reflect overall item importance and demand. Based on these categories, service levels, which are used to determine safety stock are adjusted to match appropriate business needs. The greater the demand and criticality of an object the higher the service level as there will be greater voltality in expected demand over time. This change in the service level has a ripple effect on the entire inventory model which allows for a cost based optimization problem.

Currently the project does not appropriately handle criticality as this grouping should be a measure which is quantified and replicable for regional warehouse all over the country. To do this, I am currently redefining criticality to be a measure of importance for the supply chain system where items will be more critical if they are difficult to maintain appropriate safety stock.

If you have any questions please do not hestiate to reach out!
