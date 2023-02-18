# Orders topic

The `OrderManagement` service is in charge of all CRUD operations for customer's orders. All changes will be populated via this topic contain the full entity (instead of just changes).

## GDPR notes
This topic contains GDPR sensitive information such as the customer's full name, address and the items ordered by this person.

## Schema/sample message

**Order:**

```json
{
   "name":"Alice Brown",
   "sku":"54321",
   "price":199.95,
   "shipTo":{
      "name":"Bob Brown",
      "address":"456 Oak Lane",
      "city":"Pretendville",
      "state":"HI",
      "zip":"98999"
   },
   "billTo":{
      "name":"Alice Brown",
      "address":"456 Oak Lane",
      "city":"Pretendville",
      "state":"HI",
      "zip":"98999"
   }
}
```


