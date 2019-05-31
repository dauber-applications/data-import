Order importing file format
---

**Reference Name** (required)
*No update supported*
Your internal tracking value used to refer to the job. This is commonly your purchase order number.

**Material** (required)
*No update supported*
A valid value from the following list of materials

- Asphalt
- Base
- Brush
- Cement
- Common Fill
- Compost
- Crushed Rock
- Demolished Asphalt
- Demolished Concrete [No Rebar]
- Demolished Concrete [With Rebar]
- Equipment
- Fly Ash
- Graded
- Gravel
- Haul Off
- Mag Lime
- Mulch
- Other
- Palletized Materials
- Reclaimed Asphalt Paving
- Recycled Concrete Aggregate
- Rip Rap [3x5]
- Rip Rap [6"+]
- Sand
- Select Fill
- Top Soil
- Trash

**Product Description** (required)
*Update supported*
The specific name for the product or material being provided on the job.

**Customer Name** (required)
*Update supported*
The name of the customer for the job.

**Customer GPS** (required in some cases)
*No update supported*
If the customer specified by the 'Customer Name' has not been used before, the customer's mailing location GPS must be provided for the customer to be created. This field is only required for the initial creation of new customers.

**Provider Name** (required)
*Update supported*
The name of the material/product provider for the job.

**Provider GPS** (required in some cases)
*No update supported*
If the provider specified by the 'Provider Name' has not been used before, the provider's mailing location GPS must be provided for the provider to be created. This field is only required for the initial creation of new providers.

**Provider Reference Number** (required if 'Require Ticket Information' is Yes)
*No update supported*
The number required to be shown by the driver at the point of pickup in order to load the material/product from the provider. Often referred to as a demand number.

**Unit Type** (required)
The unit type the material or product on the job is sold by.

- Cubic Yards
- Tons
- Hours
- Loads

**Unit Quantity** (required) (supports update)
*Update supported*
The quantity of product or material that is being delivered on the job.

**Remaining Quantity**
*Update supported*
If material or product has already shipped on this order, this value is used to determine the amount of product or material that should be fulfilled through Dauber.

**Skip**
*Update not applicable*
If this value is set to 'Yes', this row will be not be processed by the order importing process.

**Truck Types** (required)
*No update supported*
Set this field to 'All' if there should be no restriction on truck type when selecting trucks for load offers. If you wish to restrict truck types, specify a list of truck types separated by a comma. 

eg. 'Tandem Super,Trailer End Dump'

- All (use this value for no restrictions on truck type)
- Tandem Conventional
- Tandem Quad
- Tandem Super
- Tandem Triple
- Trailer Aluminum
- Trailer End Dump
- Trailer Belly Dump
- Trailer Live Bottom
- Trailer Round Bottom
- Trailer Side Dump
- Tanker
- Trailer Flatbed
- Tractor w/o Trailer

**Require Signature**
*No update supported*
Set this value to 'Yes' to require a signature for an Import or Export job.

**Start Date** (required)
*No update supported*
The earliest that work can be performed on the job. This is often set to the same value as the 'Auto Start Date'

**End Date**
*No update supported*
The date that all work on the job must be stopped. If you don't set this value, you can still pause or complete a job to control when work stops on a job.

**Auto Start Date**
*Update supported*
The date and time when the job should automatically started. If not specified, the order must be manually started through the administration website.

**Pickup Location Name** (required)
*Update supported*
The name of the pickup location.

**Pickup Radius**
*No update supported*
If not specified, the radius around the pickup location is set to 402 meters (1/4 of a mile). If specified, the radius of the pickup location will be set to this value in meters.

**Pickup GPS** (required)
*No update supported*
The pickup location's GPS coordinates.

eg. (30.26715, -97.743)

**Pickup Address** (required)
*No update supported*
The pickup location's address.

**Pickup City** (required)
*No update supported*
This pickup location's city.

**Pickup State** (required)
*No update supported*
The pickup location's state.

**Pickup Zip** (required)
*No update supported*
The pickup location's zip.

**Drop-off Location Name** (required)
*No update supported*
The name of the drop-off location.

**Drop-off Radius**
*No update supported*
If not specified, the radius around the drop-off location is set to 402 meters (1/4 of a mile). If specified, the radius of the drop-off location will be set to this value in meters.

**Drop-off GPS** (required)
*No update supported*
The drop-off location's GPS coordinates.

eg. (30.26715, -97.743)

**Drop-off Address** (required)
*No update supported*
The drop-off location's address.

**Drop-off City** (required)
*No update supported*
This drop-off location's city.

**Drop-off State** (required)
*No update supported*
The drop-off location's state.

**Drop-off Zip** (required)
*No update supported*
The drop-off location's zip.

**Haul Type** (required)
*No update supported*
The type of haul for the job. Import, bring material to a site from a supplier with optional tickets and a signature at the destination site. Export, remove or haul-off material from a site and dump at another location, with optional signature at pickup. Hourly, assign trucks to a site for miscellaneous work, with optional signature at beginning and end of service.

- Import
- Export
- Hourly

**Trucks** (required)
*No update supported*
If set to 'All', will allow any fleet trucks, or trucks from sub fleets to work the job. If 'Fleets' is set, only trucks from the specified list of fleets will be allowed to work the job. To specify a list of trucks that can work the job, list out the names of the trucks, separated by a comma.

eg. 'TRUCK01,TRUCK04,TRUCK17'

**Fleets** (required)
*No update supported*
If set to 'All', will allow your fleet, or any sub to work this job. To specify a list of fleets, list out the names of the fleets, separated by a comma.

eg. 'FLEET1,FLEET3,FLEET9'

**Max Trucks At Pickup**
*No update supported*
If set, when trucks are selected for a job, a job's predictions will attempt to prevent trucks at pickup from exceeding this value.

**Max Trucks At Drop-off**
*No update supported*
If set, when trucks are selected for a job, a job's predictions will attempt to prevent trucks at drop-off from exceeding this value.

**Subfleet Truck Rates**
*No update supported*
The fleet truck rates can be set at the time of import.

eg. FLEET1=5.12,FLEET09=4.15

**Pickup Notes**
Pickup notes for drivers.

**Drop-off Notes**
Drop-off notes for drivers.

**Tags**
*Update supported*
Add tags to change the way trucks are considered for job suitability. Not commonly used. 
*(These values will be provided by our engineers at the time of 
integration)*
**Excluded Tags**
*Update supported*
Add tags to change the way trucks are considered for job suitability. Not commonly used.
*(These values will be provided by our engineers at the time of 
integration)*
**Required Tags**
*Update supported*
Add tags to change the way trucks are considered for job suitability. Not commonly used.
*(These values will be provided by our engineers at the time of 
integration)*

**Bill Rate**
*Update supported*
The bill rate for the job. Must also be provided with the 'Bill Rate Unit'.

**Bill Rate Unit**
*Update supported*
The bill rate unit type for the job. Must also be provided with the 'Bill Rate'.

- Hours
- Tons
- Cubic Yards
- Loads

**Material Bill Rate**
*Update supported*
The material bill rate for the job. Must also be provided with 'Material Bill Rate Unit', 'Material Cost Rate' and 'Material Cost Rate Unit'.

**Material Bill Rate Unit**
*Update supported*
The material bill rate unit type for the job. Must also be provided with 'Material Bill Rate', 'Material Cost Rate' and 'Material Cost Rate Unit'.

- Hours
- Tons
- Cubic Yards
- Loads

**Material Cost Rate**
*Update supported*
The material cost rate for the job. Must also be provided with 'Material Bill Rate', 'Material Bill Rate Unit and 'Material Cost Rate Unit'.

**Material Cost Rate Unit**
*Update supported*
The material cost rate unit type for the job. Must also be provided with 'Material Bill Rate', 'Material Bill Rate Unit', and 'Material Cost Rate'.

- Hours
- Tons
- Cubic Yards
- Loads

**Dump Bill Rate**
*Update supported*
The dump bill rate for the job. Must also be provided with 'Dump Bill Rate Unit', 'Dump Cost Rate' and 'Dump Cost Rate Unit'.

**Dump Bill Rate Unit**
*Update supported*
The dump bill rate unit type for the job. Must also be provided with 'Dump Bill Rate', 'Dump Cost Rate' and 'Dump Cost Rate Unit'.

- Hours
- Tons
- Cubic Yards
- Loads

**Dump Cost Rate**
*Update supported*
The dump cost rate for the job. Must also be provided with 'Dump Bill Rate', 'Dump Bill Rate Unit and 'Dump Cost Rate Unit'.

**Dump Cost Rate Unit**
*Update supported*
The dump cost rate unit type for the job. Must also be provided with 'Dump Bill Rate', 'Dump Bill Rate Unit', and 'Dump Cost Rate'.

- Hours
- Tons
- Cubic Yards
- Loads
