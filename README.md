#Spree Store Demo App
---

Demo spree store.

To setup this store, please follow the following steps:

  bundle install
  rake db:create
  rake db:migrate
  rails s
  
To generate an admin account to manage the store, run:

  rake spree_auth:admin:create

Enjoy and emplore the awesome features provided by Spree

Extra:

To best thing about Spree is the flexibility. It is possible to simply use the API and backend and implement your own frontend using AngularJS or Backbone.

	rake routes
	rails c
	key = Spree::User.last.spree_api_key

Copy the ``key``, exit the console, and run:

	rails s

To test the API, visit:

	http://localhost:3000/api/products?token=<key>

Yay! Now, you get the basics of Spree, play around with it and make your own custom store. ;)