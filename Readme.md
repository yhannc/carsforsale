README
======

ID attribute values
-------------------

- **cars**
	
	Applied to a `div` tag. The list of cars in this representation. This 
	list may contain only one car.
- **makes**
	
	Applied to a `div` tag. The list of makes in this representation. This 
	list may contain only one make.
- **makeids**

	Applied to a `input` tag that can be retrieved by client-side 
	`autocomplete` javascript of 
	[jquery UI](http://code.jquery.com/ui/1.8.20/jquery-ui.min.js).
- **makenames**

	Applied to a `input` tag that can be retrieved by client-side 
	`autocomplete` javascript of 
	[jquery UI](http://code.jquery.com/ui/1.8.20/jquery-ui.min.js).
- **models**
	
	Applied to a `div` tag. The list of models in this representation. 
	This list may contain only one model.
- **modelids**

	Applied to a `input` tag that can be retrieved by client-side 
	`autocomplete` javascript of 
	[jquery UI](http://code.jquery.com/ui/1.8.20/jquery-ui.min.js).
- **modelnames**

	Applied to a `input` tag that can be retrieved by client-side 
	`autocomplete` javascript of 
	[jquery UI](http://code.jquery.com/ui/1.8.20/jquery-ui.min.js).
	
Class attribute values
----------------------

- **all**
	
	Applied to a `ul` tag. A list representation. When this element is a 
	descendant of `div.id="makes"` it may have one or more 
	`li.class="make"` descendant elements. When this element is a 
	descendant of `div.id="models"`	it may have one or more 
	`li.class="model"` descendant elements. When this element is a 
	descendant of `div.id="cars"` it may have one or more `li.class="car"` 
	descendant elements.
- **car**
	
	Applied to an `li` tag. A representation of a single car. It should 
	contain	the following descendant elements:

		a.rel="car"
- **car-add/update**
	
	Applied to a `form` tag. A link template to create or update a new 
	car profile.The element must be set to `form.method="post"` and 
	should contain the following descendant elements:
		
		input[hidden].name="item[model]"
		input[hidden].name="item[make]"
		input[text].name="item[name]"
		select.name="item[modelyear]"
		input[number].name="item[price]"
	It may also contain the following descendant elements:

		input[url].name="item[image]"
		textarea.name="item[description]"		
- **car-search**
	
	Applied to a `form` tag. A link template to search of all the cars. 
	The element must be set to `form.method="get"` and should contain 
	the following descendant elements:
		
		select.name="make"
		select.name="model"
		select.name="modelyear"
- **car-update**

	Applied to a `form` tag. A link template to update the designated 
	car's profile. The element must be set to `form.method="post"` and 
	should contain the following descendant elements:
	
		input[hidden].name="_method"
		input[text].name="item[name]"
		select.name="item[make]"
		select.name="item[model]"
		select.name="item[modelyear]"
		input[number].name="item[price]"
	It may also contain the following descendant elements:
		
		input[url].name="item[image]"
		textarea.name="item[description]"
- **control**
	
	Applied to a `div` tag. Add, update or search resources.
- **make**
	
	Applied to an `li` tag. A representation of a single make. It should 
	contain the following descendant elements:

		a.rel="make"
- **make-add/update**

	Applied to a `form` tag. A link template to create or update a new 
	make profile.The element must be set to `form.method="post"` and 
	should contain the following descendant elements:
	
		input[hidden].name="_method"
		input[text].name="item[id]"
		input[text].name="item[name]"
	It may also contain the following descendant elements:
		
		textarea.name="item[description]"
- **model**
	
	Applied to an `li` tag. A representation of a single model. It should 
	contain the following descendant elements:

		a.rel="model"
- **model-add/update**

	Applied to a `form` tag. A link template to create or update a new 
	model profile.The element must be set to `form.method="post"` and 
	should contain the following descendant elements:
	
		input[hidden].name="_method"
		input[text].name="item[id]"
		input[text].name="item[name]"
	It may also contain the following descendant elements:
		
		input[url].name="item[image]"
		textarea.name="item[description]"
- **model-search**
	
	Applied to a `form` tag. A link template to search of all the models. 
	The element must be set to `form.method="get"` and should contain 
	the following descendant elements:
		
		select.name="make"

Name attribute values
---------------------

- **item[description]**
	
	Applied to a `textarea` element. The description of a make,
	model, or car.
- **item[id]**
	
	Applied to an `input[text]` element. The id of a make, model,
	or car.
- **item[image]**
	
	Applied to an `input[url]` element. The image for a make,
	model, or car.
- **item[make]**
	
	Applied to an `input[text]`, `input[hidden]` or `select` element.
	The make of a model or car.
- **item[model]**
	
	Applied to an `input[text]`, `input[hidden]` or `select` element.
	The model of a car.
- **item[modelyear]**
	
	Applied to an `select` element. The model-year of a car.
- **item[name]**
	
	Applied to an `input[text]` element. The name of a make, 
	model, or car.
- **item[price]**
	
	Applied to an `input[number]` element. The price of a car.
- **make**
	
	Applied to a `select` element. The search value to use when 
	searching models or cars.
- **model**
	
	Applied to a `select` element. The search value to use when 
	searching cars.
- **modelyear**
	
	Applied to a `select` element. The search value to use when 
	searching cars.

Rel attribute values
--------------------

- **car**
	
	Applied to an `a` tag. A reference to a car representation.

- **make**
	
	Applied to an `a` tag. A reference to a make representation.

- **model**
	
	Applied to an `a` tag. A reference to a model representation.

Microdata types and properties
------------------------------

- **Car**

	Applied to type `Offer`
	
		itemtype="http://schema.org/Product/Car"

- **CarMake**
	
	Applied to `one-make.ejs`.

		itemtype=["http://schema.org/Organization/CarMake"](http://schema.org/Organization)
- **CarModel**
	
	Applied to `one-model.ejs`
- **Offer**
	
	Applied to `one-car.ejs`.   
