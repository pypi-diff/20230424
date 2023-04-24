# Comparing `tmp/tap_shiftbase-0.0.9.tar.gz` & `tmp/tap_shiftbase-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shiftbase-0.0.9.tar", max compression
+gzip compressed data, was "tap_shiftbase-1.0.0.tar", max compression
```

## Comparing `tap_shiftbase-0.0.9.tar` & `tap_shiftbase-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.9/README.md
--rw-r--r--   0        0        0     1078 2023-04-23 15:04:30.531566 tap_shiftbase-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.9/tap_shiftbase/__init__.py
--rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-0.0.9/tap_shiftbase/client.py
--rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentee_options.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentees.json
--rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-0.0.9/tap_shiftbase/schemas/contract_types.json
--rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-0.0.9/tap_shiftbase/schemas/custom_fields.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-0.0.9/tap_shiftbase/schemas/departments.json
--rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.9/tap_shiftbase/schemas/docs.json
--rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-0.0.9/tap_shiftbase/schemas/locations.json
--rw-r--r--   0        0        0     1609 2023-04-23 14:52:49.186296 tap_shiftbase-0.0.9/tap_shiftbase/schemas/rosters.json
--rw-r--r--   0        0        0     3699 2023-04-23 14:55:25.002146 tap_shiftbase-0.0.9/tap_shiftbase/schemas/shifts.json
--rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-0.0.9/tap_shiftbase/schemas/teams.json
--rw-r--r--   0        0        0    16267 2023-04-23 14:53:35.064834 tap_shiftbase-0.0.9/tap_shiftbase/schemas/timesheets.json
--rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-0.0.9/tap_shiftbase/schemas/users.json
--rw-r--r--   0        0        0     2455 2023-04-23 15:04:01.827316 tap_shiftbase-0.0.9/tap_shiftbase/streams.py
--rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.9/tap_shiftbase/tap.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-1.0.0/README.md
+-rw-r--r--   0        0        0     1078 2023-04-24 11:00:53.404675 tap_shiftbase-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-1.0.0/tap_shiftbase/__init__.py
+-rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-1.0.0/tap_shiftbase/client.py
+-rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentee_options.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentees.json
+-rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-1.0.0/tap_shiftbase/schemas/contract_types.json
+-rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-1.0.0/tap_shiftbase/schemas/custom_fields.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-1.0.0/tap_shiftbase/schemas/departments.json
+-rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-1.0.0/tap_shiftbase/schemas/docs.json
+-rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-1.0.0/tap_shiftbase/schemas/locations.json
+-rw-r--r--   0        0        0     5731 2023-04-24 10:57:42.043955 tap_shiftbase-1.0.0/tap_shiftbase/schemas/rosters.json
+-rw-r--r--   0        0        0     3512 2023-04-24 06:41:32.883984 tap_shiftbase-1.0.0/tap_shiftbase/schemas/shifts.json
+-rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-1.0.0/tap_shiftbase/schemas/teams.json
+-rw-r--r--   0        0        0    13203 2023-04-24 10:59:43.238525 tap_shiftbase-1.0.0/tap_shiftbase/schemas/timesheets.json
+-rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-1.0.0/tap_shiftbase/schemas/users.json
+-rw-r--r--   0        0        0     2548 2023-04-24 06:55:35.086547 tap_shiftbase-1.0.0/tap_shiftbase/streams.py
+-rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-1.0.0/tap_shiftbase/tap.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-1.0.0/PKG-INFO
```

### Comparing `tap_shiftbase-0.0.9/README.md` & `tap_shiftbase-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/pyproject.toml` & `tap_shiftbase-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shiftbase"
-version = "0.0.9"
+version = "1.0.0"
 description = "`tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "shiftbase",
 ]
```

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/client.py` & `tap_shiftbase-1.0.0/tap_shiftbase/client.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentee_options.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentee_options.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentees.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentees.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/contract_types.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/contract_types.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/custom_fields.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/custom_fields.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/departments.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/docs.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/docs.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/locations.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/rosters.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/users.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('user', OrderedDict([('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('id', OrderedDict([('type', 'string')])), ('account_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('employee_nr', OrderedDict([('type', "*

 * *                 "['string', 'null'])])), ('email', OrderedDict([('type', 'string')])), "*

 * *                 "('birthdate', OrderedDict([('type', ['string', 'null']), ('format', 'date')])), "*

 * *                 "('first_name', Orde […]*

```diff
@@ -1,88 +1,222 @@
 {
     "properties": {
-        "exchange": {
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "roster": {
+        "user": {
             "properties": {
-                "break": {
+                "account_id": {
                     "type": "string"
                 },
-                "coc": {
-                    "type": "number"
+                "age": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
-                "color": {
+                "anonymized": {
+                    "type": "boolean"
+                },
+                "avatar_150x200": {
+                    "format": "uri",
                     "type": "string"
                 },
-                "custom_fields": {
+                "avatar_15x15": {
+                    "format": "uri",
+                    "type": "string"
+                },
+                "avatar_24x24": {
+                    "format": "uri",
+                    "type": "string"
+                },
+                "avatar_30x30": {
+                    "format": "uri",
+                    "type": "string"
+                },
+                "avatar_45x45": {
+                    "format": "uri",
+                    "type": "string"
+                },
+                "avatar_60x60": {
+                    "format": "uri",
+                    "type": "string"
+                },
+                "avatar_file_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "banknr": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "birthdate": {
+                    "format": "date",
                     "type": [
                         "string",
-                        "object"
+                        "null"
                     ]
                 },
-                "date": {
+                "birthday": {
                     "format": "date",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "birthday_age": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "birthplace": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "city": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "custom_fields": {
                     "type": "string"
                 },
-                "department_id": {
+                "display_name": {
                     "type": "string"
                 },
-                "description": {
+                "email": {
                     "type": "string"
                 },
-                "endtime": {
-                    "format": "time",
+                "emergency_nr": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "employee_nr": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "enddate": {
+                    "format": "date",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "first_name": {
                     "type": "string"
                 },
-                "hide_end_time": {
+                "has_login": {
                     "type": "boolean"
                 },
-                "hours": {
-                    "type": "number"
+                "hire_date": {
+                    "format": "date",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "id": {
                     "type": "string"
                 },
-                "loaned": {
+                "invited": {
                     "type": "boolean"
                 },
-                "name": {
+                "last_login": {
+                    "format": "date-time",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "last_name": {
                     "type": "string"
                 },
-                "occurrence_id": {
+                "locale": {
                     "type": "string"
                 },
-                "published": {
+                "mfa_enabled": {
                     "type": "boolean"
                 },
-                "recurring": {
-                    "type": "boolean"
+                "mobile_nr": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "name": {
+                    "type": "string"
+                },
+                "nationality": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
-                "salary": {
-                    "type": "number"
+                "nr_of_logins": {
+                    "type": "string"
                 },
-                "shift_id": {
+                "order": {
                     "type": "string"
                 },
-                "starttime": {
-                    "format": "time",
+                "passport_number": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "phone_nr": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "plus_min_hours": {
                     "type": "string"
                 },
-                "team_id": {
+                "post_code": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "prefix": {
                     "type": "string"
                 },
-                "total": {
-                    "type": "number"
+                "roster_note": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "ssn": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
-                "user_id": {
+                "startdate": {
+                    "format": "date",
                     "type": "string"
+                },
+                "street_address": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "verified": {
+                    "type": "boolean"
                 }
             },
             "type": "object"
         }
-    },
-    "type": "object"
+    }
 }
```

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/shifts.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/shifts.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994419642857143%*

 * *Differences: {"'properties'": "{'shift': {'properties': {'break': {delete: ['description']}, 'meals': {delete: "*

 * *                 "['description']}, 'custom_fields': {delete: ['description']}}}}"}*

```diff
@@ -13,16 +13,15 @@
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "number"
                         }
-                    ],
-                    "description": "The duration of the break in minutes"
+                    ]
                 },
                 "color": {
                     "description": "The color for the shift",
                     "type": "string"
                 },
                 "created": {
                     "description": "The datetime when the shift has been created",
@@ -33,15 +32,14 @@
                 "created_by": {
                     "description": "Id of the employee that added this shift",
                     "nullable": true,
                     "readOnly": true,
                     "type": "string"
                 },
                 "custom_fields": {
-                    "description": "Custom fields that are specific for the shift",
                     "oneOf": [
                         {
                             "maxLength": 0,
                             "minLength": 0,
                             "type": "string"
                         },
                         {
@@ -91,16 +89,15 @@
                     "anyOf": [
                         {
                             "type": "integer"
                         },
                         {
                             "type": "string"
                         }
-                    ],
-                    "description": "The amount of meals"
+                    ]
                 },
                 "modified_by": {
                     "description": "Id of the employee that modified this shift",
                     "nullable": true,
                     "readOnly": true,
                     "type": "string"
                 },
```

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/teams.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/schemas/timesheets.json` & `tap_shiftbase-1.0.0/tap_shiftbase/schemas/timesheets.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999122402275304%*

 * *Differences: {"'properties'": "{'timesheet': {'properties': {'roster_id': {'type': ['string', 'null'], delete: "*

 * *                 "['description']}, 'clocked_in': {'type': ['string', 'null']}, "*

 * *                 "'clocked_in_latitude': {'type': ['string', 'null']}, 'clocked_in_longitude': "*

 * *                 "{'type': ['string', 'null']}, 'clocked_in_accuracy': {'type': ['string', "*

 * *                 "'null']}, 'clocked_in_ip': {'type': ['string', 'null']}, 'clocked_in_origin': "*

 * *                 "{'type': ['string', 'nul […]*

```diff
@@ -10,107 +10,135 @@
                             "readOnly": true,
                             "type": "string"
                         },
                         "clocked_in": {
                             "description": "Date of the clock in action",
                             "format": "date-time",
                             "nullable": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_accuracy": {
                             "description": "The accuracy of the latitude and longitude in meters",
                             "nullable": true,
                             "pattern": "^([0-9]*[.])?[0-9]+$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_ip": {
                             "description": "IP address of the clock in action",
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_latitude": {
                             "description": "Latitude of the clock in location",
                             "nullable": true,
                             "pattern": "^(\\+|-)?(?:90(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-8][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_longitude": {
                             "description": "Longitude of the clock in location",
                             "nullable": true,
                             "pattern": "^(\\+|-)?(?:180(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_origin": {
                             "description": "Origin of the clocking in action",
-                            "enum": [
-                                "terminal",
-                                "web_app",
-                                "mobile_app",
-                                "api",
-                                null
-                            ],
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_in_verified_by": {
                             "description": "User id of the employee who verified the clock in action",
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out": {
                             "description": "Date of the clock out action",
                             "format": "date-time",
                             "nullable": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_accuracy": {
                             "description": "The accuracy of the latitude and longitude in meters",
                             "nullable": true,
                             "pattern": "^([0-9]*[.])?[0-9]+$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_ip": {
                             "description": "IP address of the clock out action",
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_latitude": {
                             "description": "Latitude of the clock out location",
                             "nullable": true,
                             "pattern": "^(\\+|-)?(?:90(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-8][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_longitude": {
                             "description": "Longitude of the clock out location",
                             "nullable": true,
                             "pattern": "^(\\+|-)?(?:180(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_origin": {
                             "description": "Origin of the clocking out action",
-                            "enum": [
-                                "terminal",
-                                "web_app",
-                                "mobile_app",
-                                "api",
-                                null
-                            ],
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "clocked_out_verified_by": {
                             "description": "User id of the employee who verified the clock out action",
                             "nullable": true,
                             "readOnly": true,
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "created": {
                             "format": "date-time",
                             "readOnly": true,
                             "type": "string"
                         },
                         "created_by": {
@@ -148,81 +176,14 @@
                     ]
                 },
                 "type": "array"
             },
             "properties": {
                 "Rates": {
                     "properties": {
-                        "RateBlock": {
-                            "description": "Calculated rate blocks, the rates are split into rate blocks based on the Rate Card settings",
-                            "items": {
-                                "properties": {
-                                    "break": {
-                                        "anyOf": [
-                                            {
-                                                "nullable": true,
-                                                "type": "string"
-                                            },
-                                            {
-                                                "type": "number"
-                                            }
-                                        ],
-                                        "description": "Duration of break in minutes"
-                                    },
-                                    "date": {
-                                        "format": "date",
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "duration": {
-                                        "description": "Duration of rate block in minutes",
-                                        "type": "number"
-                                    },
-                                    "endtime": {
-                                        "description": "End time of the rate block",
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "paid_percentage": {
-                                        "description": "Surcharge of the rate block (e.g. 100, 150)",
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "paid_percentage_id": {
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "starttime": {
-                                        "description": "Start time of the rate block",
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "surcharge_pay": {
-                                        "description": "Surcharge hours (Paid)",
-                                        "type": "number"
-                                    },
-                                    "surcharge_time": {
-                                        "description": "Surcharge hours (time)",
-                                        "type": "number"
-                                    },
-                                    "time_percentage": {
-                                        "description": "Surcharge of the rate block",
-                                        "minLength": 1,
-                                        "type": "string"
-                                    },
-                                    "time_percentage_id": {
-                                        "minLength": 1,
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "type": "array",
-                            "uniqueItems": true
-                        },
                         "duration": {
                             "description": "Duration of rate in minutes",
                             "type": "number"
                         },
                         "surcharge_pay": {
                             "description": "Surcharge hours (paid)",
                             "type": "number"
@@ -263,112 +224,143 @@
                     "description": "If the timesheet is clock based",
                     "type": "boolean"
                 },
                 "clocked_break": {
                     "description": "Clocked break in minutes",
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in": {
                     "description": "Date of the clock in action",
                     "format": "date-time",
                     "nullable": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_accuracy": {
                     "description": "The accuracy of the latitude and longitude in meters",
                     "nullable": true,
                     "pattern": "^([0-9]*[.])?[0-9]+$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_ip": {
                     "description": "IP address of the clock in action",
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_latitude": {
                     "description": "Latitude of the clock in location",
                     "nullable": true,
                     "pattern": "^(\\+|-)?(?:180(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_longitude": {
                     "description": "Longitude of the clock in location",
                     "nullable": true,
                     "pattern": "^(\\+|-)?(?:180(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_origin": {
                     "description": "Origin of the clocking action",
-                    "enum": [
-                        "terminal",
-                        "web_app",
-                        "mobile_app",
-                        "api",
-                        null
-                    ],
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_in_verified_by": {
                     "description": "User id of the employee who verified the clock in action",
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out": {
                     "description": "Date of the clock out action",
                     "format": "date-time",
                     "nullable": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_accuracy": {
                     "description": "The accuracy of the latitude and longitude in meters",
                     "nullable": true,
                     "pattern": "^([0-9]*[.])?[0-9]+$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_ip": {
                     "description": "IP address of the clock out action",
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_latitude": {
                     "description": "Latitude of the clock out location",
                     "nullable": true,
                     "pattern": "^(\\+|-)?(?:90(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-8][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_longitude": {
                     "description": "Longitude of the clock out location",
                     "nullable": true,
                     "pattern": "^(\\+|-)?(?:180(?:(?:\\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\\.[0-9]{1,6})?))$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_origin": {
                     "description": "Origin of the clockout action",
-                    "enum": [
-                        "terminal",
-                        "web_app",
-                        "mobile_app",
-                        "api",
-                        null
-                    ],
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "clocked_out_verified_by": {
                     "description": "User id of the employee who verified the clock out action",
                     "nullable": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "coc": {
                     "description": "Cost to company",
                     "readOnly": true,
                     "type": "number"
                 },
                 "created": {
@@ -376,41 +368,34 @@
                     "readOnly": true,
                     "type": "string"
                 },
                 "created_by": {
                     "nullable": true,
                     "pattern": "^[0-9]+$",
                     "readOnly": true,
-                    "type": "string"
-                },
-                "custom_fields": {
-                    "anyOf": [
-                        {
-                            "items": {
-                                "type": "object"
-                            },
-                            "type": "array"
-                        },
-                        {
-                            "type": "object"
-                        }
+                    "type": [
+                        "string",
+                        "null"
                     ]
                 },
                 "date": {
                     "format": "date",
                     "type": "string"
                 },
                 "deleted": {
                     "readOnly": true,
                     "type": "boolean"
                 },
                 "endtime": {
                     "format": "time",
                     "nullable": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "id": {
                     "pattern": "^[0-9]+$",
                     "readOnly": true,
                     "type": "string"
                 },
                 "kilometers": {
@@ -420,40 +405,54 @@
                 "meals": {
                     "description": "Registered number of Meals",
                     "type": "string"
                 },
                 "modified_by": {
                     "pattern": "^[0-9]+$",
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "note": {
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "rate_card_id": {
                     "pattern": "^[0-9]+$",
                     "type": "string"
                 },
                 "reviewed": {
                     "minLength": 1,
                     "nullable": true,
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "reviewed_by": {
                     "nullable": true,
                     "pattern": "^[0-9]+$",
                     "readOnly": true,
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "roster_id": {
-                    "description": "Id of the schedule",
                     "nullable": true,
                     "pattern": "^[0-9]+$",
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "salary": {
                     "description": "Salary of the worked hours",
                     "readOnly": true,
                     "type": "number"
                 },
                 "shift_id": {
```

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/streams.py` & `tap_shiftbase-1.0.0/tap_shiftbase/streams.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,80 +9,80 @@
 from tap_shiftbase.client import shiftbaseStream
 
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 class UsersStream(shiftbaseStream):
     name = "users"
     path = "/users"
-    primary_keys = ["Users.id"]
+    primary_keys = ["user__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "users.json"
 
 class AbsenteeOptionsStream(shiftbaseStream):
     name = "absentee_options"
     path = "/absentee_options"
-    primary_keys = "absenteeoption__id"
+    primary_keys = ["absenteeoption__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "absentee_options.json"
 
 class AbsenteesStream(shiftbaseStream):
     name = "absentees"
     path = "/absentees"
-    primary_keys = ["id"]
+    primary_keys = ["absentee__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "absentees.json"
 
 class ContractTypesStream(shiftbaseStream):
     name = "contract_types"
     path = "/contract_types"
-    primary_keys = ["id"]
+    primary_keys = ["contracttype__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "contract_types.json"
 
 class CustomFieldsStream(shiftbaseStream):
     name = "custom_fields"
     path = "/custom_fields"
-    primary_keys = ["id"]
+    primary_keys = ["customfield__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "custom_fields.json"
 
 class DepartmentsStream(shiftbaseStream):
     name = "departments"
     path = "/departments"
-    primary_keys = ["id"]
+    primary_keys = ["department__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "departments.json"
 
 class LocationsStream(shiftbaseStream):
     name = "locations"
     path = "/locations"
-    primary_keys = ["id"]
+    primary_keys = ["location__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "locations.json"
 
 class RostersStream(shiftbaseStream):
     name = "rosters"
     path = "/rosters"
-    primary_keys = ["id"]
+    primary_keys = ["roster__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "rosters.json"
 
 class ShiftsStream(shiftbaseStream):
     name = "shifts"
     path = "/shifts"
-    primary_keys = ["id"]
+    primary_keys = ["shift__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "shifts.json"
 
 class TeamsStream(shiftbaseStream):
     name = "teams"
     path = "/teams"
-    primary_keys = ["id"]
+    primary_keys = ["team__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "teams.json"
 
 class TimesheetsStream(shiftbaseStream):
     name = "timesheets"
     path = "/timesheets"
-    primary_keys = ["id"]
+    primary_keys = ["timesheet__id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "timesheets.json"
```

### Comparing `tap_shiftbase-0.0.9/tap_shiftbase/tap.py` & `tap_shiftbase-1.0.0/tap_shiftbase/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.9/PKG-INFO` & `tap_shiftbase-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shiftbase
-Version: 0.0.9
+Version: 1.0.0
 Summary: `tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,shiftbase
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

