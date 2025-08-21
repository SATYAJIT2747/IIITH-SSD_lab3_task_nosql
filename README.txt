
When using MongoDB shell, the usual printjsononeline sometimes prints arrays as objects with numeric keys, like:

json
{ "0": {...}, "1": {...} }


This is not JSON format mentioned in the assignment.

hence i have used

javascript
console.log(JSON.stringify(<aggregation>.toArray()))


This prints proper arrays using [ ... ]
 Numbers appear as normal JSON numbers (not "$numberDecimal": ...)
This method was used for Tasks 5–10 to match the required output format.

