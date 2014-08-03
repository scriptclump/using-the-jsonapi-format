# jsonapi #

This allows sails to handle requests and responses via the jsonapi.org specs. For example: 
	   
```
{
 user: [{
 	id: 1,
 	name: 'Brian Jemilo II'
 },
 {
 	id: 2,
 	name: 'Mike R McNeil'
 }]
}
```

## Handling Request ##

In the policy [jsonapi.js](https://github.com/JemiloII/contribute-to-sails101/blob/master/api/policies/jsonapi.js)
If you are in need to have the resource property to be plural,

Wrap `req.body[req.options.model]` in a variable and append `+ 's'`

`resource = req.body[req.options.model] + 's';`

Then replace `req.body[req.options.model]` with `resource`

## Sending Responses ##


# Use Cases #
 
For frontend frameworks like Ember.js that heavily and unforgivingly opinionated.
	

