# Orkes Conductor

Netflix Conductor officially stopped supporting the conductor project and Orkes now maintains it.

It is almost same as the Netflix one.

The differences I found:
- Conductor spring boot app jar was readily available, whereas for Orkes conductor, I couldn't find one. Instead, they've provided a docker image which consists of the Consuctor Spring Boot app as well as the Frontend app
- Orkes Conductor also has a hosted playground
- The workflow json from Netflix conductor almost worked in Orkes conductor as it is (it required an additional field `schemaVersion`)
