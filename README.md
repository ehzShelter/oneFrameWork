# Angular 2 QuickStart Source

### glossary

######Compiler

> Angular Service which converts a Template into a Protoview. The compilation process
> involves looking for directives in the Template by matching the directives selectors
>
######Component
> Shadow dom object of you page or pages

### Change detection
> Reflects view when angular detects it

##### Component Injector
        > An component level injector which can assemble services through Dependencies Injections


#### Decorator
> a directive add behavior to the dom element. Any number of decorators can be on a DOM element. decorators can not introduce new references, views or configure application injector.

### directive

> angular attachment to HTML.
###### 3 kinds of directives

    1. Component
    2. Decorator
    3. Template

###ElementInjector

>A specialized injector which knows how to instantiate Directives. Unlike ComponentInjector the ElementInjector understands the DOM structure and can inject ancestors, parents, children, and descendants directives.

###Model(database)

>A generic concept of the source of data binding. A model can be a Directive, Service, or any other object. An object becomes a Model if it is used in a Template for data-binding.

## Proto*

>Proto* (short for prototype) prefix is a set of factories which are efficient at creating the said type. (ie ProtoView for View)
###ProtoView

>Is an internal structure which is efficient for creating View instances.
###ProtoViewPort

>Is an internal structure which is efficient for creating ViewPort instances.
#Service

>Any class which is available from application Injector.

##Template (directive)
>
>A Directive which controls the insertion of child Views into ViewPort. Only one Template directive per element.

##Template (html)

>Input to the HTML Compiler which converts the template into a set of ProtoViews.

##View

>Is a block of DOM elements which can not change structurally. (Views can only change properties on the DOM elements). Views can have ViewPorts where child Views can be added. Adding / removing Views is the only way in Angular to change the DOM structurally. An Angular application is a tree of Views.

#ViewPort

>Is a location where other Views can be attached.
