# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    A calendar would have many appointments, with the primary section having a month view and then each day rendered individually on click.

    Each day would be a component since components are meant or reusable elements.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember g component my-map
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    The component has a directory containing a template (renders the HTML/Handlebars content) and a component.js file that handles properties and actions of the component.
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
    {{my-contact contact=contact}}
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-contact/my-phone number=number}}
    ```
