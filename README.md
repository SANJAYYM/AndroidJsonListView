SimpleAndroidJsonListView
=========================

Simple JSON data parsing in android with native classes.

JSON is very light weight, structured, easy to parse and much human readable. 
JSON is best alternative to XML when your android app needs to interchange data with your server.

Sample JSON:
Following is the sample JSON that we are going to parse in this tutorial. This is very simple JSON which 
gives us list of contacts where each node contains contact information like name, email, address, gender and phone numbers.

You can get this JSON data by accessing http://api.androidhive.info/contacts/

{
    "contacts": [
        {
                "id": "c200",
                "name": "Ravi Tamada",
                "email": "ravi@gmail.com",
                "address": "xx-xx-xxxx,x - street, x - country",
                "gender" : "male",
                "phone": {
                    "mobile": "+91 0000000000",
                    "home": "00 000000",
                    "office": "00 000000"
                }
        },
        {
                "id": "c201",
                "name": "Johnny Depp",
                "email": "johnny_depp@gmail.com",
                "address": "xx-xx-xxxx,x - street, x - country",
                "gender" : "male",
                "phone": {
                    "mobile": "+91 0000000000",
                    "home": "00 000000",
                    "office": "00 000000"
                }
        },
        .
        .
        .
        .
  ]
}

The difference between [ and { - (Square brackets and Curly brackets)

In general all the JSON nodes will start with a square bracket or with a curly bracket.
The difference between [ and { is, the square bracket ([) represents starting of an JSONArray node whereas curly bracket ({) represents JSONObject. 
So while accessing these nodes we need to call appropriate method to access the data.
If your JSON node starts with [, then we should use getJSONArray() method. Same as if the node starts with {, then we should use getJSONObject() method.


refer this link for detailed description
link : http://www.androidhive.info/2012/01/android-json-parsing-tutorial/


![image1](https://github.com/ashokslsk/SimpleAndroidJsonListView/blob/master/img/1.png)
![image2](https://github.com/ashokslsk/SimpleAndroidJsonListView/blob/master/img/2.png)
![image3](https://github.com/ashokslsk/SimpleAndroidJsonListView/blob/master/img/3.png)

