# xsa-db-organisations
A simple standalone xsa db repository that contains the following objects.

|object name| type | purpose |
|----------|-----|---------|
| entities |table| a simple table with association to building|
| buildings |table| simple table |
| AddBuilding |proc| for demonstration of calling an add procedure in the parent module|
| GetEntities |proc| for demonstration of calling a get procedure in the parent module|

This micro db module will later be consumed by the companies module.

Since this is a totally standalone db module, this can have a independant application lifecycle of it's own.
All deployments should be patch incremented, so that the parent module can keep using older versions, in case of a backwards
 incompatible change in this child module is made.