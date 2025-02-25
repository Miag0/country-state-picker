# Country State Picker

NPM package to get the list of countries and their states.

[![npm version](https://badge.fury.io/js/country-state-picker.svg)](https://badge.fury.io/js/country-state-picker)

## Installation

`npm i country-state-picker --save`

## Usage

### `getCountries()`

This function will return the array of all the countries.

#### Output

```javascript
[
    {
        "name": "Afghanistan",
        "code": "af",
        "dial_code": "+93"
    },
    {
        "name": "Albania",
        "code": "al",
        "dial_code": "+355"
    },
    {
        "name": "Algeria",
        "code": "dz",
        "dial_code": "+213"
    },
    {
        "name": "Andorra",
        "code": "ad",
        "dial_code": "+376"
    }
  ...
]
```

---

### `getStates(<country_code>)`

This function will return the array of all the states of a given country.

### Example

To get the list of all the states of INDIA, the function call will look like:

```javascript
let states = getStates('in');

console.log(states)
```

#### Output

```javascript
[
    "Assam",
    "Goa",
    "Madhya Pradesh",
    "Manipur",
    "Meghalaya",
    "Mizoram",
    "National Capital Territory of Delhi",
    "Sikkim",
    "State of Andhra Pradesh",
    "State of Arunachal Pradesh",
    "State of Bihar",
    "State of Chhattisgarh",
    "State of Gujarat",
    "State of Haryana",
    "State of Himachal Pradesh",
    "State of Jammu and Kashmir",
    "State of Jharkhand",
    "State of Karnataka",
    "State of Kerala",
    "State of Maharashtra",
    "State of Nagaland",
    "State of Odisha",
    "State of Punjab",
    "State of Rajasthan",
    "State of Tamil Nad",
    "State of Uttarakhand",
    "Telangana",
    "Tripura",
    "Union Territory of Andaman and Nicobar Islands",
    "Union Territory of Chandigarh",
    "Union Territory of Dadra and Nagar Haveli",
    "Union Territory of Daman and Di",
    "Union Territory of Lakshadweep",
    "Union Territory of Puducherry",
    "Uttar Pradesh",
    "West Bengal"
]
```

### `getCountry(<country_name | country_code | dial_code>)`

This function will return the country corresponding to the argument passed.

### Example

To get the country having dial code "+91", the function call will look like:

```javascript
let country = getCountry('+91');

console.log(country)
```

#### Output

```javascript
{
    "name": "India",
    "code": "in",
    "dial_code": "+91"
}
```
