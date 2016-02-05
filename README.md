# AngularUIRouterExample

This example is updated from original with new version of bootstrap 3.3.6 

# Original Example is 
on http://ngmodules.org/modules/ui-router.


**AngularUI Router** is a routing framework for *AngularJS*, which allows you to organize the parts of your interface into a state machine. Unlike the $route service in Angular core, which is organized around URL routes, UI-Router is organized around states, which may optionally have routes, as well as other behavior, attached.

States are bound to named, nested and parallel views, allowing you to powerfully manage your application's interface.

*Warning: UI-Router is pre-beta and under active development. As such, while this library is well-tested, the API is subject to change. Using it in a project that requires guaranteed stability is not recommended.*

### Get Started
+ Get **UI-Router** in one of 4 ways: - clone & build this repository - download the release (or minified) - via Bower: by running $ bower install [angular-ui-router]() from your console - or via Component: by running $ component install [angular-ui/ui-router]() from your console

+ Include [angular-ui-router.js]() (or [angular-ui-router.min.js]()) in your index.html, after including Angular itself (For Component users: ignore this step)

+ Add **'ui.router'** to your main module's list of dependencies (For Component users: replace ['ui.router']() with require(['angular-ui-router']() )

When you're done, your setup should look similar to the following:

### Nested States & Views
The majority of UI-Router's power is in its ability to nest states & views.

+ First, follow the setup instructions detailed above.

+ Then, add a ui-view directive to the[ <body /> ]()of your app.

+ You'll notice we also added some links with ui-sref directives. In addition to managing state transitions, this directive auto-generates the href attribute of the [<a />]() element it's attached to, if the corresponding state has a URL. Next we'll add some templates. These will plug into the ui-view within [index.html](). Notice that they have their own ui-view as well! That is the key to nesting states and views.

+ Next, we'll add some child templates. These will get plugged into the ui-view of their parent state templates.

+ Finally, we'll wire it all up with $stateProvider. Set up your states in the module config, as in the following:

+ See this quick start example in action.

[Go to Quick Start Plunker for Nested States & Views](http://plnkr.co/edit/u18KQc?p=preview)
