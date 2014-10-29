mule-dbsaas-rest-project
========================

## URLs for various HTTP Operations:

```console
BASE_URL: http://localhost:8081/api
<BASE_URL>/emp  POST
<BASE_URL>/emp/<id>  GET
<BASE_URL>/emp/<id>  PUT
<BASE_URL>/emp/<id>  DEL
```

### GET - To retrieve Employee by Id
http://localhost:8081/api/emp/<empId>

### GET - To retrieve all Employees list
http://localhost:8081/api/emp/all


### POST - To create Employee details

http://localhost:8081/api/emp
* HTTP Headers: Content-Type: application/json
* Sample JSON Payload:
```console
{
    "employeeId":"901",
    "firstName":"Jane",
    "lastName": "Miller",
    "hireDate": null,
    "email": "jane.miller",
    "departmentName":"Sales"
}
```

### DELETE - To delete Employee details

http://localhost:8081/api/emp/<empId>

### PUT- To update Employee details

http://localhost:8081/api/emp/<empId>
* HTTP Headers: Content-Type: application/json


## Compiling

### Build & Compile:
```console
$mvn clean compile package
```

