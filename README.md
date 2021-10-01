# javascript-mapper
JavaScript array mapper algorithm


Write JavaScript code function that:
- Accepts an array of objects (data/records) as first input - the data input
- Accepts a key/value object as second input, to use as transformation of input's
attributes to the output attributes - the mapping
- Won't fail if no records on the data input are passed
- Won't fail if an empty mapping is passed
- The objects on the data input can have a variable number of attributes
- The returned records need to transform all input object's attributes and return
the transformed output object's attributes
- Non-mapped attributes should not be passed to the output
- Will order all results by date_modified ascending
- Will not include in the output, input records with the attribute do_not_process:
true
- If an attribute's value is an empty string, it should not be passed to the output
even if mapped
- The code needs to be optimised for performance
- The code needs to support additional custom mapping which will act based on input
field name (coded as part of the function) and will map to the output field name.
When a specific field name is encountered called "email", it will return a
different data structure. On the "email" field there is an array of email addresses
objects, and at most one has the primary_address attribute set to true. The output
is a flat field called "emailAddress", which is only set if a primary_address is
found with a valid email_address field
