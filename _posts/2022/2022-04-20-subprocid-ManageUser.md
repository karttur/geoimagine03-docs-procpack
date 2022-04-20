---
layout: subprocess
categories: subprocess
title: ManageUser
processurl: subprocid-ManageUser
rootprocid: ManageUser
subprocid: ManageUser
author: thomasg
excerpt: Add, update or remover users
date: 2022-04-20
modified: 2022-04-20
comments: true
share: true
---

#### Complete json command structure (overriding defaults)
```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "ManageUser",
      "parameters": {
        "userid": "'",
        "userpswd": "'",
        "usercat": "'",
        "firstname": "'",
        "middlename": "'",
        "lastname": "'",
        "adresssname": "'",
        "title": "'",
        "country": "'",
        "state": "'",
        "adress1": "'",
        "adress2": "'",
        "postcode": "'",
        "postcity": "'",
        "email1": "'",
        "email2": "'",
        "landline": "'",
        "mobile": "'",
        "organization": "'",
        "department": "'",
        "unit": "'",
        "position": "'"
      }
    }
  ]
}
```
#### Required json command structure (accepting all defaults)
```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "ManageUser",
      "parameters": {
        "userid": "'",
        "userpswd": "'",
        "usercat": "'",
        "lastname": "'",
        "country": "'"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | userid | text | True | ' |
| process | parameters | userpswd | text | True | ' |
| process | parameters | usercat | text | True | ' |
| process | parameters | firstname | text | False | ' |
| process | parameters | middlename | text | False | ' |
| process | parameters | lastname | text | True | ' |
| process | parameters | adresssname | text | False | ' |
| process | parameters | title | text | False | ' |
| process | parameters | country | text | True | ' |
| process | parameters | state | text | False | ' |
| process | parameters | adress1 | text | False | ' |
| process | parameters | adress2 | text | False | ' |
| process | parameters | postcode | text | False | ' |
| process | parameters | postcity | text | False | ' |
| process | parameters | email1 | text | False | ' |
| process | parameters | email2 | text | False | ' |
| process | parameters | landline | text | False | ' |
| process | parameters | mobile | text | False | ' |
| process | parameters | organization | text | False | ' |
| process | parameters | department | text | False | ' |
| process | parameters | unit | text | False | ' |
| process | parameters | position | text | False | ' |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | userid | User id |
| process | parameters | userpswd | User pass word |
| process | parameters | usercat | user category |
| process | parameters | firstname | User first name |
| process | parameters | middlename | User middle name |
| process | parameters | lastname | User last name |
| process | parameters | adresssname | User address name |
| process | parameters | title | User title |
| process | parameters | country | User country |
| process | parameters | state | User state |
| process | parameters | adress1 | User adress line 1 |
| process | parameters | adress2 | User adress line 2 |
| process | parameters | postcode | postal zip code |
| process | parameters | postcity | postal city |
| process | parameters | email1 | Primary email |
| process | parameters | email2 | Secondary email |
| process | parameters | landline | Secondary email |
| process | parameters | mobile | Secondary email |
| process | parameters | organization | User organization |
| process | parameters | department | User department |
| process | parameters | unit | User unit |
| process | parameters | position | User professional psotion |
