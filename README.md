# springboottest


git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/ak47wyh/bootRest.git
git push -u origin master



#postman

使用postman模拟请求
1.
request
localhost:8080

response

{
  "_links": {
    "persons": {
      "href": "http://localhost:8080/persons{?page,size,sort}",
      "templated": true
    },
    "profile": {
      "href": "http://localhost:8080/profile"
    }
  }
}

2.
request
localhost:8080/persons

response
{
  "_embedded": {
    "persons": [
      {
        "name": "wang1",
        "age": 1,
        "address": "shanghai1",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/1"
          },
          "person": {
            "href": "http://localhost:8080/persons/1"
          }
        }
      },
      {
        "name": "wang2",
        "age": 2,
        "address": "shanghai2",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/2"
          },
          "person": {
            "href": "http://localhost:8080/persons/2"
          }
        }
      },
      {
        "name": "wang3",
        "age": 3,
        "address": "shanghai3",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/3"
          },
          "person": {
            "href": "http://localhost:8080/persons/3"
          }
        }
      },
      {
        "name": "wang4",
        "age": 4,
        "address": "shanghai4",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/4"
          },
          "person": {
            "href": "http://localhost:8080/persons/4"
          }
        }
      },
      {
        "name": "wang5",
        "age": 5,
        "address": "shanghai5",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/5"
          },
          "person": {
            "href": "http://localhost:8080/persons/5"
          }
        }
      },
      {
        "name": "wang6",
        "age": 6,
        "address": "shanghai6",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/6"
          },
          "person": {
            "href": "http://localhost:8080/persons/6"
          }
        }
      },
      {
        "name": "wang7",
        "age": 7,
        "address": "shanghai7",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/7"
          },
          "person": {
            "href": "http://localhost:8080/persons/7"
          }
        }
      },
      {
        "name": "wang8",
        "age": 8,
        "address": "shanghai8",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/8"
          },
          "person": {
            "href": "http://localhost:8080/persons/8"
          }
        }
      },
      {
        "name": "wang",
        "age": 13,
        "address": "shanghai",
        "_links": {
          "self": {
            "href": "http://localhost:8080/persons/9"
          },
          "person": {
            "href": "http://localhost:8080/persons/9"
          }
        }
      }
    ]
  },
  "_links": {
    "self": {
      "href": "http://localhost:8080/persons{?page,size,sort}",
      "templated": true
    },
    "profile": {
      "href": "http://localhost:8080/profile/persons"
    },
    "search": {
      "href": "http://localhost:8080/persons/search"
    }
  },
  "page": {
    "size": 20,
    "totalElements": 9,
    "totalPages": 1,
    "number": 0
  }
}

3.
request
http://localhost:8080/persons/?sort=age,desc

response

{
  "_embedded" : {
    "persons" : [ {
      "name" : "wang",
      "age" : 13,
      "address" : "shanghai",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/9"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/9"
        }
      }
    }, {
      "name" : "wang8",
      "age" : 8,
      "address" : "shanghai8",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/8"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/8"
        }
      }
    }, {
      "name" : "wang7",
      "age" : 7,
      "address" : "shanghai7",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/7"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/7"
        }
      }
    }, {
      "name" : "wang6",
      "age" : 6,
      "address" : "shanghai6",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/6"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/6"
        }
      }
    }, {
      "name" : "wang5",
      "age" : 5,
      "address" : "shanghai5",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/5"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/5"
        }
      }
    }, {
      "name" : "wang4",
      "age" : 4,
      "address" : "shanghai4",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/4"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/4"
        }
      }
    }, {
      "name" : "wang3",
      "age" : 3,
      "address" : "shanghai3",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/3"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/3"
        }
      }
    }, {
      "name" : "wang2",
      "age" : 2,
      "address" : "shanghai2",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/2"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/2"
        }
      }
    }, {
      "name" : "wang1",
      "age" : 1,
      "address" : "shanghai1",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/persons/1"
        },
        "person" : {
          "href" : "http://localhost:8080/persons/1"
        }
      }
    } ]
  },
  "_links" : {
    "self" : {
      "href" : "http://localhost:8080/persons"
    },
    "profile" : {
      "href" : "http://localhost:8080/profile/persons"
    },
    "search" : {
      "href" : "http://localhost:8080/persons/search"
    }
  },
  "page" : {
    "size" : 20,
    "totalElements" : 9,
    "totalPages" : 1,
    "number" : 0
  }
}

4.
request
post body
localhost:8080/persons
{"name":"cc","address":"shanghai","age":24} 

5.
request
put body
localhost:8080/persons/10
{"name":"cc","address":"shanghai","age":20}

response
{
  "name": "cc",
  "age": 20,
  "address": "shanghai",
  "_links": {
    "self": {
      "href": "http://localhost:8080/persons/10"
    },
    "person": {
      "href": "http://localhost:8080/persons/10"
    }
  }
}

6.
request
localhost:8080/persons/10
response
#不返回任何信息