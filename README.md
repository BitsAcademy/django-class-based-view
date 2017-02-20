# django-class-based-view
### Django Class Based view
**Class-based views** are favorite feature of [Django](https://docs.djangoproject.com/),The key principles of class based view are organized and beautiful code design: don’t repeat yourself (stay **DRY**).
Whenever we see a class-based view inside a urls.py url definition, we usually see MyView.as_view().  Here __as_view__ class method does all the heavy lifting of converting our Class into a callable that the url system understands.  
**TemplateView** is a mixture of View and two mixins: __TemplateResponseMixin and ContextMixin__.
**ContextMixin** is pretty straightforward. __ContextMixin__ defines single **method get_context_data**. This returns a dictionary. It is important to become familiar with __get_context_data__ as it is one of the methods we most frequently override. A common thing to remember when overriding this method is to not forget to make the __super__ call to collect all this context.
 
#There are some great sources of information about class-based views. 
[Django Official Document](https://docs.djangoproject.com/en/1.10/topics/class-based-views/)
[Effective Django tutolrial](http://www.effectivedjango.com/classbasedviews.html)
Additionally, I find [ccbv.co.uk](http://ccbv.co.uk/) to be an invaluable resource.  It provides a flattened perspective of all of the default view types.  It is a great tool for learning how different mixins and views work together to form the complex views used in many applications.
