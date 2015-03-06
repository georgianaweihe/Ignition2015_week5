# Ignition2015_week5
Diving deeper in the MVC aspects of Rails

# Week 5: Rails MVC

#### Required 
1. Read the [Odin Project Routing Guide](http://www.theodinproject.com/ruby-on-rails/routing) and use it to <strong>answer the following questions</strong>
  1. What is the "Root" route?
    When our rails applications recieve an incoming request from the user who wants to visit the homepage of the app, root:to tells rails which controller and method(s) inside the controller to map that route too. I think of routes like an old school landline phone operator, where the user requests are taken by the operator who "translates" their request by plugging the line into the proper plug (route).
  2. What are the seven RESTful routes for a resource?
    The seven RESTful routes are the seven main types of actions we can call on a resource, each of which are comprised of/begin with/defined by one of the four basic operations of the hypertext transfer protocol (GET, POST, PUT or DELETE). The seven RESTful routes are used often so Rails has the helper method, resources :posts, which groups their seven lines of code into a single line called within config/routes.rb. The seven RESTful routes are GET 1)all the post pages, 2)just one post page, 3)a new post page, 4)an edit post page, as well as routes to create and update a users account data ie POST 5)the users data to the server and PUT 6)the users data update the server, and lastly 7) DELETE a post.
  3. Which RESTful routes share the same URL but use different verbs?
    1)GET all the post pages and 5)POST the users data to the server both submit to the same URL. The RESTful routes 2)GET a single post, 6)PUT the updates from the user on the server and 7)DELETE a post each submit to the same URL but use a different HTTP verb.
  4. How do you specify an ID or other variable in a route?
    You can specify an ID or other variable by prepending the field with a colon.
  5. How can you easily write all seven RESTful routes in Rails?
    As I mentioned above, the seven RESTful routes are seven lines of code (for each route) that can be called in Rails using the single line helper method, resources :posts, in config/routes.rb
  6. What is the Rails helper method that creates the HTML for links?
    The link(underscore)to helper method lets you create links. In order to do so, you call the name of the method followed by the "text or title" that you want the user to see and lastly a path or URL. The URL can be written explicitly or we can use the path helper method to generate a path when link to method is called.
2. Read the [Odin Project Controller Guide](http://www.theodinproject.com/ruby-on-rails/controllers)
3. Read the [Odin Project Views Guide](http://www.theodinproject.com/ruby-on-rails/views) and use it to <strong>answer the following questions</strong>
  1. What is a layout?
  2. What's the difference between a "view template" and a "layout"?
  3. What is a "Preprocessor"?
  4. Why are preprocessors useful?
  5. How do you make sure a preprocessor runs on your file?
  6. What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?
  7. What is the difference between the <%= and <% tags?
  8. What is a view partial?
  9. How do you insert a partial into your view?
  10. How can you tell that a view file is a partial?
  11. How do you pass a local variable to a partial?
  12. What's the magical Rails shortcut for rendering a User? A bunch of Users?
  13. What are asset tags and why are they used?
4. (By Monday 3/9) By yourself, complete the [Odin Project: Basic Routes, Views and Controllers](http://www.theodinproject.com/ruby-on-rails/basic-routes-views-and-controllers)
  1. Skip step 1 of the Application Skeleton section.  As we did last week, you will:
    1. Create a new Rails workspace on C9
    2. Add `/.c9` to your `.gitignore` file
    3. Setup git and commit the project:
      1. `git init`
      2. `git add .`
      3. `git commit -m 'initial commit'`
    4. Create a new repo on GitHub without a `README` or `.gitignore`
    5. Add your remote and push to github (replace the `<username>` and `<repo>` with your username and repo name)
      1. `git remote add origin https://github.com/<username>/<repo>.git`
      2. `git push -u origin master`
5. (By Thursday 3/12) As a group, complete the Rails tutorial [Chapter 5](https://www.railstutorial.org/book/filling_in_the_layout#top). Make sure to trade off coding, one person should not write everything.  
  1. Pick up where you left on your week 4 assignment with your new partner.  One person should be new to the codebase, one should have been working on it the previous week.

#### Optional
- Read the [Rails Guide on Routing](http://guides.rubyonrails.org/routing.html)
- Read the [Rails Guide on Controllers](http://guides.rubyonrails.org/action_controller_overview.html)
- Read the [Rails Guide on Layouts](http://guides.rubyonrails.org/layouts_and_rendering.html)
- Read the [Odin Project Guide on Asset Pipelines](http://www.theodinproject.com/ruby-on-rails/the-asset-pipeline)
