# vue-anyblok-components

A set of Vue.js components for Anyblok based projects.
We choose to go with Bulma and Buefy for as base ui components.

The vue anyblok components can extends Buefy components or not, and if css styling is used it's recommend to use Bulma. 
They are designed against an http rest json api, that can be given by anyblok_pyramid_rest_api or your own implementation.
On the components part, we use Axios to manage http call.

# Components

* [TODO] - vac-errors - Display api errors message
* [TODO] - vac-record-create - Facilities to subit a form and create a new record through a POST
* [TODO] - vac-record-update - Facilities to update a record and submit the form through PUT or PATCH
* [TODO] - vac-record-read-only - Facilitlies to display a record in a form but read only
* [TODO] - vac-record-delete - Button to delete a record
* [TODO] - vac-records-filters - Search and/or filter component, that helps to reduce a list of records depending on record field or presistant tags (that represents complex filter query)
* [TODO] - vac-records-actions - Facilities to select some records and execute a common action on them
* [TODO] - vac-records-list - Display a list of records (GET collection)
* [TODO] - vac-records-browse - Facilities to navigate through a list of pages (records)

# Maybe in the future
* [TODO] - vac-records-calendar 
* [TODO] - vac-records-kanban 

# Contribute to vue-anyblok-components

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Run your unit tests
```
npm run test:unit
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
