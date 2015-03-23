#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- What is the "Root" route?

When our rails applications recieve an incoming request from the user who wants to visit the homepage of the app, root:to tells rails which controller and method(s) inside the controller to map that route too. I think of routes like an old school landline phone operator, where the user requests are taken by the operator who "translates" their request by plugging the line into the proper plug (route).


- What are the seven RESTful routes for a resource?

The seven RESTful routes are the seven main types of actions we can call on a resource, each of which are comprised of/begin with/defined by one of the four basic operations of the hypertext transfer protocol (GET, POST, PUT or DELETE). The seven RESTful routes are used often so Rails has the helper method, resources :posts, which groups their seven lines of code into a single line called within config/routes.rb. The seven RESTful routes are GET 1)all the post pages ie "index", 2)just one post page ie "show", 3)a new post page ie "new", 4)an edit post page ie "edit", as well as routes to create and update a users account data ie POST 5)the users data to the server ie "create" and PUT 6)the users data update the server ie "update", and lastly 7) DELETE a post ie "destroy".


- Which RESTful routes share the same URL but use different verbs?

1)GET all the post pages and 5)POST the users data to the server both submit to the same URL. The RESTful routes 2)GET a single post, 6)PUT the updates from the user on the server and 7)DELETE a post each submit to the same URL but use a different HTTP verb.

- How do you specify an ID or other variable in a route?

You can specify an ID or other variable by prepending the field with a colon.

- How can you easily write all seven RESTful routes in Rails?

As I mentioned above, the seven RESTful routes are seven lines of code (for each route) that can be called in Rails using the single line helper method, resources :posts, in config/routes.rb

- What is the Rails helper method that creates the HTML for links?

The link _ to helper method lets you create links. In order to do so, you call the name of the method followed by the "text or title" that you want the user to see and lastly a path or URL. The URL can be written explicitly or we can use the path helper method to generate a path when link to method is called.

##### Odin Project Views Guide Questions:
- What is a layout?

A layout contains the basic HTML structures such as html and body tags and code to load javascript and css files. Thus, layouts are "basically just a shell around the individual page" which contain anything needed across all your webpages. ("Views", The Odin Project)

- What's the difference between a "view template" and a "layout"?

View templates are a collection of partials and HTML that dynamically change based on your route call.

- What is a "Preprocessor"?

A preprocessor executes the file on the server (including the ERB) in order to send a finalized HTML file to the browser.

- Why are preprocessors useful?

Preprocessing allows you to code dynamically within HTML.

- How do you make sure a preprocessor runs on your file?

Extensions on file names such as ".html.erb" and ".css.scss", which we have used before, instruct Rails to preprocess before sending it off to the browser.

- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?

The outputted filetype of a preprocessed *.html.erb file is a regular HTML file, and *.css.scss is a regular CSS file.

- What is the difference between the <%= and <% tags?

<%= tags are going to execute the embedded Ruby code and return something that will be displayed in the HTML template, such as instance variables. The <% tags will also execute embedded Ruby code but will not return anything to display in the HTML file that is sent to the browser.

- What is a view partial?

It is a partial section of a view template that can be shared by other files, allowing the user to organize and reuse similar code wherever it may be needed.

- How do you insert a partial into your view?

In your app/views folder, you can write a view partial file then call it in whatever view templates you need it in.

- How can you tell that a view file is a partial?

Partials can be recognized bu their name--the file is named according to the directory it can be found under, then the underscored file name is fitted with the proper extension designation (like ".html.erb").

- How do you pass a local variable to a partial?

You should explicitly pass it by losing the @ and using the :locals key options hash in the render method.

- What's the magical Rails shortcut for rendering a User? A bunch of Users?

You can tell Rails to render the User directly rather than making it into its own partial. Call a for @users.each loop and inside the loop, render user. To render a bunch of users, the line " render @users " will suffice.

- What are asset tags and why are they used?

Asset tags grab images and will render their proper HTML tag for you.

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<linkhere>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](<linkhere>)
