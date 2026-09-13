### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

```
url:localhost:8000/movie/
method:POST
body:{
"title":"BKU",
"year":2026,
"language":"malayalam",
"run_time":167
}

```
`http_request for list all movie`

```
url:localhost:8000/movie/
method:GET
```
`http_request for fetching movie detail`

```
url:localhost:8000/movie/4/
method:GET

```
`http_request for update movie`

```
url:localhost:8000/movie/4/
method:PUT
body:{
"title":"Athiradi",
"year":2026,
"language":"malayalam",
"run_time":160
}
```
`http_request for delete movie`

```
url:localhost:8000/movie/5/
method:DELETE

```

### HOSPITAL REGISTER MANAGEMENT TASK
---

```

hospital

id   patient_name  phone_no      assigned_doc      consultation_fee


1          Alia     9746756743      george          160
2          mick     8757389874      cam             200
3          aysha    7467393746      samuel          800
4          liam     9837647374      ron             450
5          daniel   8736541537      manu            180


```

` http request to add a patient register `

```

url:localhost:8000/hospital/
method:POST
body:{

    "patient_name":"Anjali",
    "phone_no":9367428777,
    "assigned_doc:"Hari",
    "consultation_fee":180

}

```
---

` http request to list all  patient registers `

```
url:localhost:8000/hospital/
method:GET
```

`http_request for fetching a petient register detail`

```
url:localhost:8000/hospital/3
method:GET

```

`http_request for update patient register`

```

url:localhost:8000/hospital/2
method:PUT
body:{

    "patient_name":"hiba",
    "phone_no":9367477345,
    "assigned_doc:"george",
    "consultation_fee":160

}

```


`http_request for delete a patient record`

```
url:localhost:8000/hospital/5/
method:DELETE

```



### Expense 


id        Date       Category       Amount      payment_method
1         12/04/26     Food           360           UPI
2         13/04/26    Transport       120           Cash
3         14/04/26    Shopping        850           Card
4         15/04/26    Food            250           UPI
5         16/04/26    Entertainment   500           Card
6         17/04/26    Bills           1200          UPI
7         18/04/26    Transport       180           Cash
8         19/04/26    Groceries       1450          UPI
9         20/04/26    Food            420           Card



`http_request for adding a record to expense `

```
url:localhost:8000/expenses/
method:POST
body:{
    "Date":"21/04/26",
    "Category":"Transport",
    "Amount":2000,
    "payment_method":Card
}

```

` http_request for listing the entire records of expense`

```
url:localhost:8000/expenses/
method:GET
```


` http_request for listing record of a specific id `

```
url:localhost:8000/expenses/{id}/
method:GET

```

`http_request for updating a record`

```
url:localhost:8000/expenses/{5}/
method:PUT
body:{

    "Date":"18/04/26",
    "Category":"Food",
    "Amount":678,
    payment_method:"UPI"

}
```

` http_request for deleting a record`

```
url:localhost:8000/expenses/{id}/
method:DELETE

```