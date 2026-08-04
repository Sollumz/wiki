# Car Generators

Car generators define spawn points where vehicles can appear.

They are represented using the following model:

<figure><img src="../../.gitbook/assets/image (111).png" alt="" width="375"><figcaption><p>Model used by car generators</p></figcaption></figure>

All car generators properties and functionality can be found in the Car Generators tab panel in the sidebar.

<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption><p>Car Generators tab panel</p></figcaption></figure>

Each car generator entry is linked to a **Collection**. Each object inside this collection defines a spawn location. All objects in the collection share the same car generator properties.

#### Operators

<table><thead><tr><th width="313.333251953125"></th><th>Description</th></tr></thead><tbody><tr><td><strong>Create Car Generator Object</strong></td><td>Create an object at the cursor location with the car generator model and add to the linked collection.</td></tr><tr><td><strong>Select All Car Generator Objects</strong></td><td>Select all objects in the linked collection.</td></tr></tbody></table>

#### **Properties**

<table><thead><tr><th width="192.6666259765625">Property</th><th>Description</th></tr></thead><tbody><tr><td><strong>Name</strong></td><td>Label used to identify this car generator entry. For UI display/organization purposes only, has no effect on export or in-game. If empty, a label will be automatically generated based on the other settings.</td></tr><tr><td><strong>Model</strong></td><td>Use a specific vehicle model.</td></tr><tr><td><strong>Model Set</strong></td><td>Use any vehicle model found in the specified model set. Model sets are defined in vehiclemodelsets.meta</td></tr><tr><td><strong>Creation Rule</strong></td><td></td></tr><tr><td><strong>Flags</strong></td><td></td></tr><tr><td><strong>Livery</strong></td><td></td></tr><tr><td><strong>Body Color Remap</strong></td><td></td></tr></tbody></table>

***

When a car generator object is selected you can view its properties in the "Sollumz > Map Cargen Properties" panel in the object properties tab.

<figure><img src="../../.gitbook/assets/image (112).png" alt="" width="375"><figcaption><p>Car generator properties of the selected object</p></figcaption></figure>

The "View in Sidebar" button synchronizes the selection in the Entities list with the selected objects in the scene.

"Move to New Collection" can be used when you want to change the properties of only the selected car generator objects. Remember, the properties shown here are shared by all objects in the collection. This button creates a new car generator entry, a new collection, and moves the selected objects to this collection. Then, you can modify the properties without affecting the other car generators.
