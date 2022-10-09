---
sidebar_position: 1
---

# List Students


**_POSTMAN DOC URL;_**

[https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-da3ea7c3-6310-4363-9645-758526190405](https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-da3ea7c3-6310-4363-9645-758526190405)


### Request

**_Path;_**

`/api/student/lists?from=10.10.2020 00:00&to=10.10.2021 23:59&per_page=15&current_page=1`

`from`: register date, examples: `10.10.2020 00:00` or `10.10.2020` (**required**),

`to`: register date, examples: `10.10.2021 23:59` or `10.10.2021`  (**required**),

`per_page`: min 1 max 25 (optional default=10),

`current_page` or `student_lists`: min 1 (optional default=1)

**_Method: `GET`_**

### Response

**_Successful result;_**
```json
{
  "state": "true",
  "data": {
    "current_page": 2,
    "data": [
      {
        "id": 13383,
        "register_date": 1415829600,
        "student_id": "13383GAL14-15BAH-ING999",
        "institution_id": 1681123,
        "branch_id": 1705123,
        "subject_id": 1710123,
        "group_id": 1711123,
        "type": "1",
        "state": "1",
        "name": "Example",
        "surname": "Student",
        "identity": "11111111111",
        "mobile": "",
        "mail": ""
      },
      {
        "id": 13382,
        "register_date": 1415829600,
        "student_id": "13382GAL14-15BAH-ING123",
        "institution_id": 1681123,
        "branch_id": 1705123,
        "subject_id": 1710123,
        "group_id": 1711123,
        "type": "1",
        "state": "1",
        "name": "Example2",
        "surname": "Student",
        "identity": "11111111111",
        "mail": ""
      }
    ],
    "first_page_url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=1",
    "from": 3,
    "last_page": 5,
    "last_page_url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=5",
    "links": [
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=1",
        "label": "pagination.previous",
        "active": false
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=1",
        "label": "1",
        "active": false
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=2",
        "label": "2",
        "active": true
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=3",
        "label": "3",
        "active": false
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=4",
        "label": "4",
        "active": false
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=5",
        "label": "5",
        "active": false
      },
      {
        "url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=3",
        "label": "pagination.next",
        "active": false
      }
    ],
    "next_page_url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=3",
    "path": "http://galata-egitim.delta-course.net/api/student/lists",
    "per_page": 2,
    "prev_page_url": "http://galata-egitim.delta-course.net/api/student/lists?from=10.10.2020&to=1650585600&per_page=2&student_lists=1",
    "to": 4,
    "total": 9,
    "maps": {
      "type": {
        "1": "Registered Students",
        "6": "Pre-registered(Not Registered) Students"
      },
      "state": [
        "Passive",
        "Active",
        "Frozen",
        "Canceled",
        "Expired"
      ]
    }
  }
}
```

## MAPS

Result items can be understood by MAPS.

```json
  "maps": {
      "type": {
        "1": "Registered Students",
        "6": "Pre-registered(Not Registered) Students"
      },
      "state": [
        "Passive",
        "Active",
        "Frozen",
        "Canceled",
        "Expired"
      ]
    }
```


## Code Examples


It can be taken from: [https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-da3ea7c3-6310-4363-9645-758526190405](https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-da3ea7c3-6310-4363-9645-758526190405)